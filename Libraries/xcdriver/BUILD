load("@bazel_skylib//rules:copy_file.bzl", "copy_file")

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

copy_file(
    name = "xcodebuild_bin",
    src = ":xcbuild",
    out = "xcodebuild",
    allow_symlink = True,
    visibility = ["//visibility:public"],
)
