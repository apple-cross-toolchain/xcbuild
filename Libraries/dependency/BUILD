cc_library(
    name = "dependency",
    srcs = glob(["Sources/**/*.cpp"]),
    hdrs = glob(["Headers/**/*.h"]),
    includes = ["Headers"],
    visibility = ["//Libraries:__subpackages__"],
    deps = [
        "//Libraries/ext",
        "//Libraries/libutil",
    ],
)

cc_binary(
    name = "dependency-info-tool",
    srcs = ["Tools/dependency-info-tool.cpp"],
    deps = [
        ":dependency",
        "//Libraries/process",
    ],
)

cc_binary(
    name = "dump_dependency",
    srcs = ["Tools/dump_dependency.cpp"],
    deps = [
        ":dependency",
        "//Libraries/process",
    ],
)
