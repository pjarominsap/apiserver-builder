package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["anytoken_test.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiserver/plugin/pkg/authenticator/token/anytoken",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = ["anytoken.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiserver/plugin/pkg/authenticator/token/anytoken",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library"],
)
