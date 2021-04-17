cc_library(
    name = "xcsdk",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
        "//Libraries/process",
        "@zlib",
    ],
)

cc_binary(
    name = "xcode-select",
    srcs = ["Tools/xcode-select.cpp"],
    deps = [
        ":xcsdk",
        "@zlib",
    ],
)

cc_binary(
    name = "xcrun",
    srcs = ["Tools/xcrun.cpp"],
    deps = [":xcsdk"],
)
