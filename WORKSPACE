load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "libxml",
    build_file = "//ThirdParty:libxml.BUILD",
    sha256 = "f63c5e7d30362ed28b38bfa1ac6313f9a80230720b7fb6c80575eeab3ff5900c",
    strip_prefix = "libxml2-2.9.7",
    urls = [
        "https://mirror.bazel.build/xmlsoft.org/sources/libxml2-2.9.7.tar.gz",
        "http://xmlsoft.org/sources/libxml2-2.9.7.tar.gz",
    ],
)

http_archive(
    name = "zlib",
    build_file = "//ThirdParty:zlib.BUILD",
    sha256 = "c3e5e9fdd5004dcb542feda5ee4f0ff0744628baf8ed2dd5d66f8ca1197cb1a1",
    strip_prefix = "zlib-1.2.11",
    urls = [
        "https://zlib.net/zlib-1.2.11.tar.gz",
    ],
)

http_archive(
    name = "libpng",
    build_file = "//ThirdParty:libpng.BUILD",
    sha256 = "7f415186d38ca71c23058386d7cf5135c8beda821ee1beecdc2a7a26c0356615",
    strip_prefix = "libpng-1.2.57",
    urls = [
        "https://github.com/glennrp/libpng/archive/v1.2.57.tar.gz",
    ],
)

http_archive(
    name = "linenoise",
    build_file = "//ThirdParty:linenoise.BUILD",
    sha256 = "1086f82fbf30b0618b1953b05d33db62c68fc7ce49391ce1374192f776fde72d",
    strip_prefix = "linenoise-97d2850af13c339369093b78abe5265845d78220",
    urls = [
        "https://github.com/antirez/linenoise/archive/97d2850af13c339369093b78abe5265845d78220.tar.gz",
    ],
)
