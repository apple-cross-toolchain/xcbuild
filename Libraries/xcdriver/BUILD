cc_library(
    name = "xcdriver",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/builtin",
        "//Libraries/libutil",
        "//Libraries/pbxbuild",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
        "//Libraries/process",
        "//Libraries/xcexecution",
        "//Libraries/xcformatter",
        "//Libraries/xcsdk",
        "//Libraries/xcworkspace",
    ],
)

cc_binary(
    name = "xcbuild",
    srcs = ["Tools/xcbuild.cpp"],
    deps = [":xcdriver"],
)
