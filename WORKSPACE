workspace(name = "SEMoonbase")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

# Load platformio_rules
git_repository(
    name = "platformio_rules",
    remote = "http://github.com/mum4k/platformio_rules.git",
    tag = "v0.0.14",
)

load("@platformio_rules//bazel:deps.bzl", "platformio_rules_dependencies")

platformio_rules_dependencies()

load("@platformio_rules//bazel:transitive.bzl", "platformio_rules_transitive_dependencies")

platformio_rules_transitive_dependencies()

load("@platformio_rules//bazel:pip_parse.bzl", "platformio_rules_pip_parse_dependencies")

platformio_rules_pip_parse_dependencies()

load("@platformio_rules//bazel:pip_install.bzl", "platformio_rules_pip_install_dependencies")

platformio_rules_pip_install_dependencies()
