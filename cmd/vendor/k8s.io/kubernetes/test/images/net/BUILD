package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
)

go_binary(
    name = "net",
    importpath = "k8s.io/kubernetes/test/images/net",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    importpath = "k8s.io/kubernetes/test/images/net",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/kubernetes/test/images/net/common:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/test/images/net/nat:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//test/images/net/common:all-srcs",
        "//test/images/net/nat:all-srcs",
    ],
    tags = ["automanaged"],
)
