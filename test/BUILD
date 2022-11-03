load("@rules_python//python:defs.bzl", "py_binary")

package(default_visibility = ["//visibility:public"])

py_binary(
    name = "test_grpc",
    srcs = ["test_grpc.py"],
    deps = [
        "//proto:py_info_proto",
        # "//proto:py_api_grpc",
    ],
)
