package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["rand_test.go"],
    importpath = "k8s.io/apimachinery/pkg/util/rand",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = ["rand.go"],
    importpath = "k8s.io/apimachinery/pkg/util/rand",
    tags = ["automanaged"],
)
