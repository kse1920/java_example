package(default_visibility = ["//visibility:public"])

# Used by Bazel. If a test program depends on this target, it is
# assumed to be sharding-compliant.
exports_files(["test_sharding_compliant"])

filegroup(
    name = "srcs",
    srcs = glob(["**"]) + [
        "//tools/build_defs:srcs"
    ]
)

filegroup(
    name = "embedded_tools_srcs",
    srcs = glob(["**"]) + [
        "//tools/build_defs:embedded_tools"
    ]
)

test_suite(
    name = "all_windows_tests",
    tests = [
        "//tools/build_defs:all_windows_tests"
    ]
    visibility = ["//src:__pkg__"]
)
