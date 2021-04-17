cc_library(
    name = "libutil",
    srcs = glob([
        "Sources/**/*.c",
        "Sources/**/*.cpp",
    ]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = ["//Libraries/ext"],
)
