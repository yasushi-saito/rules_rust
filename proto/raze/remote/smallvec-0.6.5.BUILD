"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//proto/raze", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

# Unsupported target "bench" with type "bench" omitted

rust_library(
    name = "smallvec",
    srcs = glob(["**/*.rs"]),
    crate_features = [
        "default",
        "std",
    ],
    crate_root = "lib.rs",
    crate_type = "lib",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.6.5",
    deps = [
        "@raze__unreachable__1_0_0//:unreachable",
    ],
)
