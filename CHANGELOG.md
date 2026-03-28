# Changelog

## v0.1.4

**Enterprise Font Subsetting (DAG IPC)**

- **Hermetic & Cache-Safe:** `fluent-zero-build` now natively leverages Cargo's Inter-Package Communication (IPC) to aggregate character sets across all nested dependencies.
- **No More Scraping:** Replaces brittle `cargo_metadata` workspace-walking with a 100% `sccache`, `Bazel`, and `Nix` compatible build pipeline.

**⚠️ Migration & Setup:** Dependency crates must now declare a globally unique `links` key in their `Cargo.toml`. Please see the **Enterprise Font Subsetting (DAG IPC)** section in the [README.md](README.md) for full instructions and a copy-paste Python subsetter script template.

## v0.1.3

New `FluentZeroBuilder` API for generating charset, allowing easy font subsetting.

## v0.1.2

Small, miscellaneous documentation improvements and fixes.

## v0.1.1

Hotfix:

- add shields to the README.md
- link to the source code repository and docs.rs documentation from the Cargo.toml metadata.
