cc_library(
    name = "libcar",
    srcs = glob([
        "Sources/**/*.c",
        "Sources/**/*.cpp",
    ]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/ext",
        "//Libraries/libbom",
        "@zlib",
    ],
)

cc_binary(
    name = "dump_car",
    srcs = ["Tools/dump_car.cpp"],
    deps = [
        ":libcar",
        "//Libraries/graphics",
    ],
)
