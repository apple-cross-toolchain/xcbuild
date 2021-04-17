cc_library(
    name = "pbxsetting",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/plist",
        "//Libraries/process",
    ],
)

cc_binary(
    name = "dump_xcconfig",
    srcs = ["Tools/dump_xcconfig.cpp"],
    deps = [":pbxsetting"],
)
