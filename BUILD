load("@bazel_gazelle//:def.bzl", "gazelle")
load("@io_tweag_rules_haskell//haskell:haskell.bzl", "haskell_toolchain")

# gazelle:prefix github.com/TokTok
# gazelle:exclude go-toxcore-c/tools
# gazelle:exclude jvm-toxcore-c
gazelle(
    name = "gazelle",
    command = "fix",
    extra_args = [
        "-build_file_name",
        "BUILD",
    ],
    prefix = "github.com/TokTok",
)

haskell_toolchain(
    name = "ghc",
    tools = "@my_ghc//:bin",
    version = "8.0.1",
)
