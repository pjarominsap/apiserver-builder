package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["validation.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/kube-aggregator/pkg/apis/apiregistration/validation",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/api/validation:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/api/validation/path:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/validation:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//cmd/vendor/k8s.io/kube-aggregator/pkg/apis/apiregistration:go_default_library",
    ],
)
