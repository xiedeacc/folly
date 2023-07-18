load("@rules_cc//cc:defs.bzl", "cc_library")
load("@rules_foreign_cc//foreign_cc:configure.bzl", "configure_make", "configure_make_variant")
load("@bazel_skylib//lib:selects.bzl", "selects")

filegroup(
    name = "all",
    srcs = glob(
        ["**"],
        exclude = [],
    ),
    visibility = ["//visibility:public"],
)

configure_make_variant(
    name = "jemalloc_build",
    args = ["-j8"],
    autogen = True,
    autogen_options = [],
    configure_in_place = True,
    configure_options = [
        "--enable-static",
        "--enable-prof",
        "--enable-prof-libunwind",
    ],
    copts = [
        "-D_GNU_SOURCE",
        "-D_REENTRANT",
        "-g3",
        "-O3",
        "-funroll-loops",
        "-fvisibility=hidden",
        "-Wall",
        "-Wextra",
        "-Wimplicit-fallthrough",
        "-Wsign-compare",
        "-Wundef",
        "-Wno-format-zero-length",
        "-Wpointer-arith",
        "-Wno-missing-braces",
        "-Wno-missing-field-initializers",
        "-Wno-missing-attributes",
        "-pipe",
    ],
    lib_source = ":all",
    linkopts = [
        "-lunwind",
    ],
    out_static_libs = ["libjemalloc.a"],
    toolchain = "@rules_foreign_cc//toolchains:preinstalled_make_toolchain",
)

cc_library(
    name = "jemalloc",
    visibility = ["//visibility:public"],
    deps = [
        ":jemalloc_build",
    ],
)
