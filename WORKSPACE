workspace(name = "bazel_python_bug")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

# Python
rules_python_version = "6b6aedda3aab264dc1e27470655e0ae0cfb2b5bc"

git_repository(
    name = "io_bazel_rules_python",
    remote = "https://github.com/bazelbuild/rules_python.git",
    commit = rules_python_version
    )

load("@io_bazel_rules_python//python:pip.bzl", "pip_repositories", "pip_import")
pip_repositories()

pip_import(
    name="pip",
    requirements="//:requirements.txt"
    )
load("@pip//:requirements.bzl", "pip_install")
pip_install()