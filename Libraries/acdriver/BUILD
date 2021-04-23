cc_library(
    name = "acdriver",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/dependency",
        "//Libraries/ext",
        "//Libraries/graphics",
        "//Libraries/libbom",
        "//Libraries/libcar",
        "//Libraries/libutil",
        "//Libraries/plist",
        "//Libraries/process",
        "//Libraries/xcassets",
    ],
)

cc_binary(
    name = "actool",
    srcs = ["Tools/actool.cpp"],
    visibility = ["//visibility:public"],
    deps = [":acdriver"],
)
