load("@io_bazel_rules_python//python:python.bzl", "py_binary", "py_library")
load("@pip//:requirements.bzl", "requirement")

py_binary(
    name="main",
    srcs=["main.py"],
    deps=[
        # requirement("tensorflow"),
        # requirement("tensorflow_transform"),
        requirement("apache_beam[gcp]"),
    ]
)