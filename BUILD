package(default_visibility = ["//visibility:public"])

load("@rules_proto_grpc//python:defs.bzl", "python_grpc_library")

python_grpc_library(
    name = "google_a_py_grpc",
    deps = [
        "@proto//google/nested:a_proto",
    ],
)

py_binary(
    name = "foo",
    srcs = [":foo.py"],
    deps = [
        ":google_a_py_grpc",
    ],
)

python_grpc_library(
    name = "ok_a_py_grpc",
    deps = [
        "@proto//base/nested:a_proto",
    ],
)

py_binary(
    name = "bar",
    srcs = [":bar.py"],
    deps = [
        ":ok_a_py_grpc",
    ],
)
