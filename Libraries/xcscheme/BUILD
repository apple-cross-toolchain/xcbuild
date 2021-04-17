cc_library(
    name = "xcscheme",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/libutil",
        "//Libraries/pbxsetting",
        "//Libraries/plist",
    ],
)
