package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "expansion.go",
        "lister.go",
        "tags.go",
    ],
    importpath = "k8s.io/kubernetes/cmd/libs/go2idl/lister-gen/generators",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/gengo/args:go_default_library",
        "//cmd/vendor/k8s.io/gengo/generator:go_default_library",
        "//cmd/vendor/k8s.io/gengo/namer:go_default_library",
        "//cmd/vendor/k8s.io/gengo/types:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/cmd/libs/go2idl/client-gen/types:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
