package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
)

go_binary(
    name = "genfeddocs",
    importpath = "k8s.io/kubernetes/federation/cmd/genfeddocs",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = ["gen_fed_docs.go"],
    importpath = "k8s.io/kubernetes/federation/cmd/genfeddocs",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/spf13/cobra/doc:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/cmd/genutils:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/federation/cmd/federation-apiserver/app:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/federation/cmd/federation-controller-manager/app:go_default_library",
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
