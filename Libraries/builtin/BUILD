cc_library(
    name = "builtin",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    linkopts = select({
        "@platforms//os:macos": [
            "-framework",
            "CoreFoundation",
            "-framework",
            "CoreServices",
        ],
        "//conditions:default": [],
    }),
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/dependency",
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
    ],
)

cc_binary(
    name = "builtin-copy",
    srcs = ["Tools/copy.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-copyPlist",
    srcs = ["Tools/copyPlist.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-copyStrings",
    srcs = ["Tools/copyStrings.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-copyTiff",
    srcs = ["Tools/copyTiff.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-embeddedBinaryValidationUtility",
    srcs = ["Tools/embeddedBinaryValidationUtility.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-infoPlistUtility",
    srcs = ["Tools/infoPlistUtility.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-lsRegisterURL",
    srcs = ["Tools/lsRegisterURL.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-productPackagingUtility",
    srcs = ["Tools/productPackagingUtility.cpp"],
    deps = [":builtin"],
)

cc_binary(
    name = "builtin-validationUtility",
    srcs = ["Tools/validationUtility.cpp"],
    deps = [":builtin"],
)
