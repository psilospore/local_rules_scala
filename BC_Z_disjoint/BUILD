load("@io_bazel_rules_scala//scala/bloop:scala_with_bloop.bzl", "scala_binary", "scala_library")
## TODO
scala_binary(
    name = "C_run",
    srcs = glob(["C.scala"]),
    main_class = "ABC.C",
    visibility = ["//visibility:public"],
    deps = ["C", "B"]
)

scala_library(
    name = "C",
    srcs = glob(["C.scala"]),
    visibility = ["//visibility:public"],
    deps = ["B"]
)

scala_library(
    name = "B",
    srcs = glob(["B.scala"]),
    visibility = ["//visibility:public"]
)

scala_library(
    name = "Z",
    srcs = glob(["Z.scala"]),
    visibility = ["//visibility:public"]
)

scala_library(
    name = "Z_run",
    srcs = glob(["Z_run.scala"]),
    visibility = ["//visibility:public"],
    deps = ["Z"]
)