package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["errors_test.go"],
    importpath = "k8s.io/apimachinery/pkg/util/errors",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "errors.go",
    ],
    importpath = "k8s.io/apimachinery/pkg/util/errors",
    tags = ["automanaged"],
)
