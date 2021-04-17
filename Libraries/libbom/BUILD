cc_library(
    name = "libbom",
    srcs = glob(["Sources/**/*.c"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
    ],
)

cc_binary(
    name = "dump_bom",
    srcs = ["Tools/dump_bom.c"],
    deps = [":libbom"],
)

cc_binary(
    name = "lsbom",
    srcs = ["Tools/lsbom.cpp"],
    deps = [":libbom"],
)
