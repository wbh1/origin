package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "fake_mirror_client.go",
        "mock_manager.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubelet/pod/testing",
    deps = [
        "//pkg/kubelet/checkpoint:go_default_library",
        "//pkg/kubelet/checkpointmanager:go_default_library",
        "//pkg/kubelet/container:go_default_library",
        "//pkg/kubelet/types:go_default_library",
        "//vendor/github.com/stretchr/testify/mock:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
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
