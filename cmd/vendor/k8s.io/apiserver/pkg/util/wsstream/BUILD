package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = [
        "conn_test.go",
        "stream_test.go",
    ],
    importpath = "k8s.io/apiserver/pkg/util/wsstream",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/golang.org/x/net/websocket:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "conn.go",
        "doc.go",
        "stream.go",
    ],
    importpath = "k8s.io/apiserver/pkg/util/wsstream",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//vendor/golang.org/x/net/websocket:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
    ],
)
