package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["fuzzer.go"],
    importpath = "k8s.io/kubernetes/cmd/kubeadm/app/apis/kubeadm/fuzzer",
    tags = ["automanaged"],
    deps = [
        "//vendor/github.com/google/gofuzz:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/api/testing:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/cmd/kubeadm/app/apis/kubeadm:go_default_library",
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
