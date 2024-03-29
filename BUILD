load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "folly",
    srcs = glob(
        [
            "folly/**/*.cpp",
            "folly/**/*.S",
        ],
        exclude = [
            "folly/docs/**",
            "folly/build/**",
            "folly/logging/example/**",
            "folly/test/**/*.cpp",
            "folly/**/test/**/*.cpp",
            "folly/**/*Test.cpp",
            "folly/python/**/*.cpp",
        ],
    ),
    hdrs = glob(
        [
            "folly/**/*.h",
        ],
        exclude = [
            "folly/test/**/*.h",
            "folly/**/test/**/*.h",
            "folly/python/**/*.h",
        ],
    ),
    copts = [
        "-iquote external/libdwarf/src/libdwarf",
        "-isystem .",
        "-Wall",
        "-Wno-deprecated",
        "-Wno-deprecated-declarations",
        "-Wno-sign-compare",
        "-Wno-unused",
        "-Wunused-label",
        "-Wunused-result",
        "-Wuninitialized",
        "-faligned-new",
        "-Wshadow-compatible-local",
        "-Wno-noexcept-type",
        "-std=c++17",
        "-fPIC",
        "-finput-charset=UTF-8",
        "-fsigned-char",
        "-fopenmp",
        "-faligned-new",
        "-fcoroutines",
        "-msse4.2",
        "-mpclmul",
        "-mavx",
        "-mavx2",
    ],
    includes = [
        "external/com_github_google_snappy",
        "external/com_github_libevent_libevent",
        "external/double-conversion",
        "external/org_bzip_bzip2",
        "external/zlib",
    ],
    linkopts = [
        "-pthread",
        "-ldl",
        "-lstdc++",
    ],
    linkstatic = True,
    local_defines = [
        "_GNU_SOURCE",
        "_REENTRANT",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "@boost//:algorithm",
        "@boost//:context",
        "@boost//:crc",
        "@boost//:filesystem",
        "@boost//:multi_index",
        "@boost//:preprocessor",
        "@boost//:program_options",
        "@com_github_facebook_zstd//:libzstd",
        "@com_github_fmtlib_fmt//:fmt",
        "@com_github_gflags_gflags//:gflags",
        "@com_github_glog_glog//:glog",
        "@com_github_google_snappy//:snappy",
        "@com_github_libevent_libevent//:libevent",
        "@double-conversion//:double-conversion",
        "@jemalloc",
        "@libdwarf//:dwarf",
        "@libsodium",
        "@libunwind//:unwind",
        "@lzma",
        "@openssl//:ssl",
        "@org_bzip_bzip2//:libbzip2",
        "@zlib",
    ],
    alwayslink = True,
)
