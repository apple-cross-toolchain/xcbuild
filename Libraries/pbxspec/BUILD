cc_library(
    name = "pbxspec",
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
        "//Libraries/ext",
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
    ],
)

cc_binary(
    name = "dump_xcspec",
    srcs = ["Tools/dump_xcspec.cpp"],
    deps = [":pbxspec"],
)
