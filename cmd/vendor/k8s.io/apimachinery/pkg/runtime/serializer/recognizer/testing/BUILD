package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["recognizer_test.go"],
    importpath = "k8s.io/apimachinery/pkg/runtime/serializer/recognizer/testing",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/serializer/json:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/serializer/recognizer:go_default_library",
    ],
)
