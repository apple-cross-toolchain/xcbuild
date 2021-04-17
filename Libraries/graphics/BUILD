cc_library(
    name = "graphics",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    linkopts = select({
        "@platforms//os:macos": [
            "-framework",
            "CoreFoundation",
            "-framework",
            "CoreServices",
            "-framework",
            "ImageIO",
        ],
        "//conditions:default": [],
    }),
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/ext",
        "@libpng",
        "@zlib",
    ],
)
