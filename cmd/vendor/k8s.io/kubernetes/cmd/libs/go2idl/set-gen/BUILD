package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
)

go_binary(
    name = "set-gen",
    importpath = "k8s.io/kubernetes/cmd/libs/go2idl/set-gen",
    library = ":go_default_library",
    tags = ["automanaged"],
)

exports_files([
    "types.go",
])

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    importpath = "k8s.io/kubernetes/cmd/libs/go2idl/set-gen",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/gengo/args:go_default_library",
        "//cmd/vendor/k8s.io/gengo/examples/set-gen/generators:go_default_library",
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
