package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["pathrecorder_test.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiserver/pkg/server/mux",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/github.com/stretchr/testify/assert:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "pathrecorder.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiserver/pkg/server/mux",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
    ],
)
