package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["validation_test.go"],
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/k8s.io/apiserver/pkg/apis/audit:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = ["validation.go"],
    tags = ["automanaged"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/apis/audit:go_default_library",
    ],
)
