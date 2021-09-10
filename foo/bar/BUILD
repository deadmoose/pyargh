package(default_visibility = ["//visibility:public"])

load("@rules_python//python:defs.bzl", "py_library")
load("@rules_python//python:defs.bzl", "py_test")

py_library(
    name = "bar",
    srcs = glob(
        ["*.py"],
        exclude = ["*_test.py"],
    ),
)

py_test(
    name = "baz_test",
    srcs = ["baz_test.py"],
    deps = [":bar"],
)
