cc_library(
    name = "xcworkspace",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
        "//Libraries/process",
    ],
)

cc_binary(
    name = "dump_xcworkspace",
    srcs = ["Tools/dump_xcworkspace.cpp"],
    deps = [
        ":xcworkspace",
        "//Libraries/pbxproj",
        "//Libraries/xcscheme",
    ],
)
