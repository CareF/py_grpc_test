load("@rules_proto_grpc//cpp:defs.bzl", "cpp_grpc_library")
load("@rules_proto_grpc//python:defs.bzl", "python_grpc_library")
load("@com_google_protobuf//:protobuf.bzl", "py_proto_library")

package(default_visibility = ["//visibility:public"])

proto_library(
    name = "info_proto",
    srcs = ["info.proto"],
)

py_proto_library(
    name = "py_info_proto",
    srcs = ["info.proto"],
)

proto_library(
    name = "api_proto",
    srcs = ["api.proto"],
    deps = [":info_proto"],
)

cpp_grpc_library(
    name = "cc_api_grpc",
    protos = [":api_proto"],
)

python_grpc_library(
    name = "py_api_grpc",
    protos = [":api_proto"],
)

