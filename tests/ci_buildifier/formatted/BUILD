load("@rules_python//python:defs.bzl", "py_binary", "py_library")

py_library(
    name = "hello_lib",
    srcs = ["hello_lib.py"],
    visibility = ["//visibility:public"],
)

py_binary(
    name = "main1",
    srcs = ["main.py"],
    deps = [
        ":hello_lib",
    ],
)
