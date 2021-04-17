cc_library(
    name = "pbxbuild",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/dependency",
        "//Libraries/ext",
        "//Libraries/libutil",
        "//Libraries/pbxproj",
        "//Libraries/pbxsetting",
        "//Libraries/pbxspec",
        "//Libraries/plist",
        "//Libraries/process",
        "//Libraries/xcscheme",
        "//Libraries/xcsdk",
        "//Libraries/xcworkspace",
    ],
)

cc_binary(
    name = "dump_hmap",
    srcs = ["Tools/dump_hmap.cpp"],
    deps = [":pbxbuild"],
)
