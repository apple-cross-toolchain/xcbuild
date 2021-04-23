load("@rules_pkg//:pkg.bzl", "pkg_tar")

pkg_tar(
    name = "xcbuild",
    srcs = [
        "//Libraries/acdriver:actool",
        "//Libraries/plist:PlistBuddy",
        "//Libraries/plist:plutil",
        "//Libraries/xcdriver:xcodebuild",
        "//Libraries/xcsdk:xcode-select",
        "//Libraries/xcsdk:xcrun",
    ],
    extension = "tar.xz",
)
