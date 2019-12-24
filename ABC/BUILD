load("@rules_scala_annex//rules:scala.bzl", "scala_binary", "scala_library")

scala_binary(
    name = "C_run",
    srcs = glob(["C.scala"]),
    visibility = ["//visibility:public"],
    deps = ["C"]
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