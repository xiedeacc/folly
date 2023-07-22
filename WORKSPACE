workspace(name = "folly")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository", "new_git_repository")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "platforms",
    sha256 = "d62cb553b378d2acb4e63de21dce82d025ce2ef2bdfcee2c2b742788314df0b1",
    strip_prefix = "platforms-0.0.2",
    urls = [
        "https://github.com/xiedeacc/platforms/archive/0.0.2.tar.gz",
    ],
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "f795b82792edeb03a7a060a908bc2cfc9702273b1387479fb99d208e83a3d7ad",
    strip_prefix = "bazel-gazelle-v0.24.0",
    urls = [
        "https://github.com/xiedeacc/bazel-gazelle/-/archive/v0.24.0/bazel-gazelle-v0.24.0.tar.gz",
    ],
)

http_archive(
    name = "bazel_skylib",
    sha256 = "3b620033ca48fcd6f5ef2ac85e0f6ec5639605fa2f627968490e52fc91a9932f",
    strip_prefix = "bazel-skylib-1.3.0",
    urls = [
        "https://github.com/xiedeacc/bazel-skylib/-/archive/1.3.0/bazel-skylib-1.3.0.tar.gz",
    ],
)

load("@bazel_skylib//lib:versions.bzl", "versions")

versions.check("5.2.0")

http_archive(
    name = "rules_cc",
    sha256 = "af6cc82d87db94585bceeda2561cb8a9d55ad435318ccb4ddfee18a43580fb5d",
    strip_prefix = "rules_cc-0.0.4",
    urls = [
        "https://github.com/xiedeacc/rules_cc/-/archive/0.0.4/rules_cc-0.0.4.tar.gz",
    ],
)

http_archive(
    name = "rules_foreign_cc",
    sha256 = "c7527231b3e10643efc6add713311e8eb4f707a5a8f3835fc2d335db5fbe7217",
    strip_prefix = "rules_foreign_cc-fe3c552dda3a1f5d31ed6014ba6229a5a9283161",
    urls = [
        "https://github.com/xiedeacc/rules_foreign_cc/-/archive/fe3c552dda3a1f5d31ed6014ba6229a5a9283161/rules_foreign_cc-fe3c552dda3a1f5d31ed6014ba6229a5a9283161.tar.gz",
    ],
)

load("@rules_foreign_cc//foreign_cc:repositories.bzl", "rules_foreign_cc_dependencies")

http_archive(
    name = "rules_proto",
    sha256 = "9850fcf6ad40fa348e6f13b2cfef4bb4639762f804794f2bf61d988f4ba0dae9",
    strip_prefix = "rules_proto-4.0.0-3.19.2-2",
    urls = [
        "https://github.com/xiedeacc/rules_proto/-/archive/4.0.0-3.19.2-2/rules_proto-4.0.0-3.19.2-2.tar.gz",
    ],
)

load("@rules_proto//proto:repositories.bzl", "rules_proto_dependencies", "rules_proto_toolchains")

http_archive(
    name = "rules_perl",
    sha256 = "0f234dbaf4acacee9e131a117c8b02bc8910724427ec8e3d69df5e3b36899477",
    strip_prefix = "rules_perl-ca8ea624afc939bdb70100ac8d609d2b8d81308c",
    urls = [
        "https://github.com/xiedeacc/rules_perl/-/archive/ca8ea624afc939bdb70100ac8d609d2b8d81308c/rules_perl-ca8ea624afc939bdb70100ac8d609d2b8d81308c.tar.gz",
    ],
)

load("@rules_perl//perl:deps.bzl", "perl_register_toolchains")

perl_register_toolchains()

http_archive(
    name = "rules_python",
    sha256 = "94750828b18044533e98a129003b6a68001204038dc4749f40b195b24c38f49f",
    strip_prefix = "rules_python-0.21.0",
    urls = [
        "https://github.com/xiedeacc/rules_python/-/archive/0.21.0/rules_python-0.21.0.tar.gz",
    ],
)

http_archive(
    name = "rules_java",
    sha256 = "7436356107f1cf24b45f95909753e521efe2d06622de184ea25e13cb7a0d72f9",
    strip_prefix = "rules_java-5.5.0",
    urls = [
        "https://github.com/xiedeacc/rules_java/-/archive/5.5.0/rules_java-5.5.0.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_rules_swift",
    sha256 = "104b16612b1084918d58083b3ee2f6521eb202b4502019870da7351d10a4777f",
    strip_prefix = "rules_swift-1.5.1",
    urls = [
        "https://github.com/xiedeacc/rules_swift/-/archive/1.5.1/rules_swift-1.5.1.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_rules_apple",
    sha256 = "d6735ed25754dbcb4fce38e6d72c55b55f6afa91408e0b72f1357640b88bb49c",
    strip_prefix = "rules_apple-0.31.3",
    urls = [
        "https://github.com/xiedeacc/rules_apple/-/archive/0.31.3/rules_apple-0.31.3.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_apple_support",
    sha256 = "c02a8c902f405e5ea12b815f426fbe429bc39a2628b290e50703d956d40f5542",
    strip_prefix = "apple_support-0.10.0",
    urls = [
        "https://github.com/xiedeacc/apple_support/-/archive/0.10.0/apple_support-0.10.0.tar.gz",
    ],
)

http_archive(
    name = "io_bazel_rules_docker",
    sha256 = "91844808532e5ce316b3c010929493c0244f3d37593afd6de04f71821d5136d9",
    strip_prefix = "rules_docker-v0.9.0",
    urls = [
        "https://github.com/xiedeacc/rules_docker/-/archive/v0.9.0/rules_docker-v0.9.0.tar.gz",
    ],
)

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "5169057086cacb107e0c8e8430f90b17518fc8052e1ab0ce25cbc227287f1cd4",
    strip_prefix = "rules_go-b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2",
    urls = [
        "https://github.com/xiedeacc/rules_go/-/archive/b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2/rules_go-b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2.tar.gz",
    ],
)

load("@io_bazel_rules_go//go:deps.bzl", "go_register_toolchains", "go_rules_dependencies")

http_archive(
    name = "rules_pkg",
    sha256 = "d258fb6965cf3d7ebdbe146ec7e28b605f0644cb880101604e166e35d4ca62bc",
    strip_prefix = "rules_pkg-0.7.1",
    url = "https://github.com/xiedeacc/rules_pkg/-/archive/0.7.1/rules_pkg-0.7.1.tar.gz",
)

load("@rules_pkg//:deps.bzl", "rules_pkg_dependencies")

http_archive(
    name = "rules_jvm_external",
    sha256 = "f36441aa876c4f6427bfb2d1f2d723b48e9d930b62662bf723ddfb8fc80f0140",
    strip_prefix = "rules_jvm_external-4.1",
    urls = ["https://github.com/xiedeacc//rules_jvm_external/-/archive/4.1/rules_jvm_external-4.1.tar.gz"],
)

http_archive(
    name = "com_grail_bazel_compdb",
    sha256 = "d32835b26dd35aad8fd0ba0d712265df6565a3ad860d39e4c01ad41059ea7eda",
    strip_prefix = "bazel-compilation-database-0.5.2",
    urls = [
        "https://github.com/xiedeacc/bazel-compilation-database/-/archive/0.5.2/bazel-compilation-database-0.5.2.tar.gz",
    ],
)

load("@com_grail_bazel_compdb//:deps.bzl", "bazel_compdb_deps")

http_archive(
    name = "cpplint",
    build_file = "//bazel:cpplint.BUILD",
    sha256 = "ddc50661b62103376675d6e4bcaa85745fa523343c3d93a1f774685005f9afb3",
    strip_prefix = "cpplint-1.6.0",
    urls = [
        "https://github.com/xiedeacc/cpplint/-/archive/1.6.0/cpplint-1.6.0.tar.gz",
    ],
)

http_archive(
    name = "jemalloc",
    sha256 = "0f1e76ece7d0828122ac18139c9760dc4778097fb0b5d2ae9016781c98117644",
    strip_prefix = "jemalloc-9cfab520be9eb97a094bba8e1d2d32f632082194",
    urls = [
        "https://github.com/xiedeacc/jemalloc/archive/9cfab520be9eb97a094bba8e1d2d32f632082194.tar.gz",
    ],
)

http_archive(
    name = "zlib",
    sha256 = "976fbac5738f73852ec867da32278d618db709260a608c61ef23c0be87c24cc9",
    strip_prefix = "zlib-75e6f80e8ad4e51cd2ee729771111323268ff210",
    urls = [
        "https://github.com/xiedeacc/zlib/archive/75e6f80e8ad4e51cd2ee729771111323268ff210.tar.gz",
    ],
)

http_archive(
    name = "org_bzip_bzip2",
    sha256 = "647a04c5a216fb89543ec8086ca2dd91773bf52f35e34d5a9df83417a291a387",
    strip_prefix = "bzip2-fcba92ced7426b2b772741f526cfc4ae6269ef72",
    urls = [
        "https://github.com/xiedeacc/bzip2/archive/fcba92ced7426b2b772741f526cfc4ae6269ef72.tar.gz",
    ],
)

http_archive(
    name = "org_lzma_lzma",
    sha256 = "accf5897c8b2ba51a33194e8f59694f385b46ebd5ee74d5d37002bbccf810727",
    strip_prefix = "xz-7c02e2ef6809801867a1a466a89398b19f959ed9",
    urls = [
        "https://github.com/xiedeacc/xz/archive/7c02e2ef6809801867a1a466a89398b19f959ed9.tar.gz",
    ],
)

http_archive(
    name = "lz4",
    sha256 = "1c85f0f25c653fd2e9483746a7d1f4b9deefe440e50b350705243f7181b5bcbf",
    strip_prefix = "lz4-a403c95fab5dcaf04ee33d9fe46807241838d0a9",
    urls = [
        "https://github.com/xiedeacc/lz4/archive/a403c95fab5dcaf04ee33d9fe46807241838d0a9.tar.gz",
    ],
)

http_archive(
    name = "com_github_facebook_zstd",
    sha256 = "7d7522bfbc9644d2a9d5acddb9018e21b1f0ef0298d2d5b910102d72c58a2838",
    strip_prefix = "zstd-43e30c7e358af7141499f782d9df1462c9cf644d",
    urls = [
        "https://github.com/xiedeacc/zstd/archive/43e30c7e358af7141499f782d9df1462c9cf644d.tar.gz",
    ],
)

http_archive(
    name = "openssl",
    build_file = "//bazel:openssl.BUILD",
    repo_mapping = {
        "@com_github_madler_zlib": "@zlib",
    },
    sha256 = "e2f8d84b523eecd06c7be7626830370300fbcc15386bf5142d72758f6963ebc6",
    strip_prefix = "openssl-1.1.1u",
    urls = [
        "https://github.com/openssl/openssl/releases/download/OpenSSL_1_1_1u/openssl-1.1.1u.tar.gz",
    ],
)

http_archive(
    name = "com_github_libevent_libevent",
    sha256 = "0b2fd93d207404a978a084e3a16cceda02a0d30f698fe8b5d4e9572050c2a6ce",
    strip_prefix = "libevent-139ec3083a767978fc8bc873fe8f4eaba611976c",
    urls = [
        "https://github.com/xiedeacc/libevent/archive/139ec3083a767978fc8bc873fe8f4eaba611976c.tar.gz",
    ],
)

http_archive(
    name = "com_github_fmtlib_fmt",
    sha256 = "97292e726aefc36f84d0c9fec48158e5aa1341a84664892df3e4661890227f68",
    strip_prefix = "fmt-bf065c46f13e394a48456ee137e7e2847d824e2d",
    urls = [
        "https://github.com/xiedeacc/fmt/archive/bf065c46f13e394a48456ee137e7e2847d824e2d.tar.gz",
    ],
)

http_archive(
    name = "com_github_gflags_gflags",
    sha256 = "f9859e5026509ef7db263166ad739db8b8ad6ec34ce3faecc2619d1f56ff25fb",
    strip_prefix = "gflags-v2.2.2",
    urls = [
        "https://github.com/xiedeacc/gflags/-/archive/v2.2.2/gflags-v2.2.2.tar.gz",
    ],
)

http_archive(
    name = "com_github_glog_glog",
    sha256 = "06751251e75b28bf80ae1e582468b84382eccf4cfa1a9cc0761fb35ba21c65a1",
    strip_prefix = "glog-v0.5.0",
    urls = [
        "https://github.com/xiedeacc/glog/-/archive/v0.5.0/glog-v0.5.0.tar.gz",
    ],
)

http_archive(
    name = "com_github_google_snappy",
    sha256 = "b91e28142b8693aff5a8fbde2ca942fc9c6ec320d5004b0b399ee5c49bb6448a",
    strip_prefix = "snappy-27f34a580be4a3becf5f8c0cba13433f53c21337",
    urls = [
        "https://github.com/xiedeacc/snappy/archive/27f34a580be4a3becf5f8c0cba13433f53c21337.tar.gz",
    ],
)

http_archive(
    name = "double-conversion",
    sha256 = "d745263abfc7f973b6d7e1890feda2a4323307797a2218345f22b29379b476d3",
    strip_prefix = "double-conversion-29e61b7f6ed92c8809d78f96c7cb59cd293adce8",
    urls = [
        "https://github.com/xiedeacc/double-conversion/archive/29e61b7f6ed92c8809d78f96c7cb59cd293adce8.tar.gz",
    ],
)

http_archive(
    name = "libunwind",
    sha256 = "e273318b5c514cb63b0036202f571a1da6c685803eef4f38c2179f35069a1b",
    strip_prefix = "libunwind-707805705cb28fad69c3cc19d9e9c5aded3af104",
    urls = [
        "https://github.com/xiedeacc/libunwind/archive/707805705cb28fad69c3cc19d9e9c5aded3af104.tar.gz",
    ],
)

rules_foreign_cc_dependencies()

rules_proto_dependencies()

rules_proto_toolchains()

go_rules_dependencies()

go_register_toolchains(version = "1.18")

rules_pkg_dependencies()

bazel_compdb_deps()
