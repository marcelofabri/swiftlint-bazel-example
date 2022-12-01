load("@com_github_buildbuddy_io_rules_xcodeproj//xcodeproj:defs.bzl", "xcodeproj")

filegroup(
    name = "extra_rules",
    srcs = glob(["**/*.swift"]),
    visibility = ["//visibility:public"],
)

xcodeproj(
    name = "swiftlint_xcodeproj",
    build_mode = "bazel",
    project_name = "SwiftLint",
    tags = ["manual"],
    top_level_targets = [
        "@SwiftLint//:swiftlint",
        "@SwiftLint//Tests:ExtraRulesTests",
    ],
)
