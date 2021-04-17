cc_library(
    name = "pbxproj",
    srcs = glob([
        "Sources/**/*.cpp",
        "PrivateHeaders/**/*.h",
    ]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = [
        "Headers",
        "PrivateHeaders",
    ],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
    ],
)

cc_binary(
    name = "dump_xcodeproj",
    srcs = ["Tools/dump_xcodeproj.cpp"],
    deps = [
        ":pbxproj",
        "//Libraries/xcscheme",
    ],
)
