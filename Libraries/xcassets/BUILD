cc_library(
    name = "xcassets",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/ext",
        "//Libraries/libutil",
        "//Libraries/plist",
    ],
)

cc_binary(
    name = "dump_xcassets",
    srcs = ["Tools/dump_xcassets.cpp"],
    deps = [":xcassets"],
)
