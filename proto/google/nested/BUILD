package(default_visibility = ["//visibility:public"])

load("@rules_proto//proto:defs.bzl", "proto_library")

proto_library(
    name = "b_proto",
    srcs = ["b.proto"],
)

proto_library(
    name = "a_proto",
    srcs = ["a.proto"],
    deps = [":b_proto"],
)
