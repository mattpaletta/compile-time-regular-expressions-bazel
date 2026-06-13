load("//:ctre.bzl", "ctre_tests")
load("@rules_cc//cc:defs.bzl", "cc_library")

cc_library(
    name = "ctre",
    hdrs = glob(["include/**/*.hpp"]),
    deps = [],
    includes = ["include"],
    copts = ["-std=c++20"],
    visibility = ["//visibility:public"],
)

ctre_tests(
    name = "ctre_tests",
    srcs = glob(["tests/*.cpp"]),
    deps = [
        ":ctre",
    ],
)
