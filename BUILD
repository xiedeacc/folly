load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "folly",
    srcs = glob(
        ["folly/**/*.cpp"],
        exclude = [
            "folly/docs/**",
            "folly/build/**",
            "folly/logging/example/**",
            "folly/Benchmark.cpp",
            "folly/test/**/*.cpp",
            "folly/**/test/**/*.cpp",
            "folly/**/*Test.cpp",
            "folly/python/**/*.cpp",
        ],
    ),
    hdrs = glob(
        [
            "folly/*.h",
            "folly/**/*.h",
            "folly/experimental/*.h",
        ],
        exclude = [
            "folly/test/**/*.h",
            "folly/**/test/**/*.h",
            "folly/python/**/*.h",
        ],
    ),
    copts = [
        "-isystem .",
        "-std=gnu++1z",
        "-fPIC",
        "-finput-charset=UTF-8",
        "-fsigned-char",
        "-fopenmp",
        "-faligned-new",
        "-Wall",
        "-Wno-deprecated",
        "-Wno-deprecated-declarations",
        "-Wno-sign-compare",
        "-Wno-unused",
        "-Wunused-label",
        "-Wunused-result",
        "-Wshadow-compatible-local",
        "-Wno-noexcept-type",
        "-mpclmul",
    ],
    linkopts = [
        "-pthread",
        "-ldl",
        "-lstdc++fs",
    ],
    linkstatic = True,
    visibility = ["//visibility:public"],
    deps = [
        "@com_github_facebook_zstd//:libzstd",
        "@com_github_fmtlib_fmt//:fmt",
        "@com_github_gflags_gflags//:gflags",
        "@com_github_glog_glog//:glog",
        "@com_github_google_snappy//:snappy",
        "@double-conversion//:double-conversion",
        "@jemalloc",
        #"@openssl//:ssl",
        "@org_bzip_bzip2//:libbzip2",
        "@org_lzma_lzma//:liblzma",
        "@zlib",
    ],
)

#cc_library(
#name = "follybenchmark",
#srcs = ["folly/Benchmark.cpp"],
#copts = [
#"-std=gnu++1z",
#"-fPIC",
#"-finput-charset=UTF-8",
#"-fsigned-char",
#"-fopenmp",
#"-faligned-new",
#"-Wall",
#"-Wno-deprecated",
#"-Wno-deprecated-declarations",
#"-Wno-sign-compare",
#"-Wno-unused",
#"-Wunused-label",
#"-Wunused-result",
#"-Wshadow-compatible-local",
#"-Wno-noexcept-type",
#"-mpclmul",
#],
#deps = [
#":folly",
#],
#)
