workspace(name = "example")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "build_bazel_rules_swift",
    sha256 = "8407fa0fd04a7ce1d6bb95e90b216404466f809eda459c23cb57b5fa1ef9d639",
    url = "https://github.com/bazelbuild/rules_swift/releases/download/0.21.0/rules_swift.0.21.0.tar.gz",
)

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:extras.bzl",
    "swift_rules_extra_dependencies",
)

swift_rules_extra_dependencies()

new_local_repository(
    name = "homebrew_arm64",
    path = "/opt/homebrew",
    build_file = "BUILD.homebrew"
)

new_local_repository(
    name = "homebrew_x86_64",
    path = "/usr/local/homebrew",
    build_file = "BUILD.homebrew"
)
