cc_library(
    name = "xcformatter",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/pbxbuild",
        "//Libraries/pbxproj",
        "//Libraries/pbxsetting",
    ],
)
