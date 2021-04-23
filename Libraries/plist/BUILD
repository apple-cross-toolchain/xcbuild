cc_library(
    name = "plist",
    srcs = glob([
        "PrivateHeaders/**/*.h",
        "Sources/**/*.cpp",
        "Sources/**/*.h",
        "Sources/**/*.c",
    ]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = [
        "Headers",
        "PrivateHeaders",
    ],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/process",
        "@libxml",
    ],
)

cc_binary(
    name = "PlistBuddy",
    srcs = ["Tools/PlistBuddy.cpp"],
    copts = ["-DHAVE_LINENOISE"],
    visibility = ["//visibility:public"],
    deps = [
        ":plist",
        "@linenoise",
    ],
)

cc_binary(
    name = "plutil",
    srcs = ["Tools/plutil.cpp"],
    visibility = ["//visibility:public"],
    deps = [":plist"],
)
