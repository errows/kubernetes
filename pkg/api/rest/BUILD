package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "create.go",
        "delete.go",
        "doc.go",
        "export.go",
        "rest.go",
        "types.go",
        "update.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/errors:go_default_library",
        "//pkg/api/meta:go_default_library",
        "//pkg/api/validation/genericvalidation:go_default_library",
        "//pkg/api/validation/path:go_default_library",
        "//pkg/apis/meta/v1:go_default_library",
        "//pkg/genericapiserver/api/request:go_default_library",
        "//pkg/runtime:go_default_library",
        "//pkg/runtime/schema:go_default_library",
        "//pkg/util/validation/field:go_default_library",
        "//pkg/watch:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//pkg/api/rest/resttest:all-srcs",
    ],
    tags = ["automanaged"],
)
