load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_binary", "scala_test")

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
    visibility = ["//visibility:public"],
    deps = ["A"]
)

scala_library(
    name = "A",
    srcs = glob(["A.scala"]),
    visibility = ["//visibility:public"]
)