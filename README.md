# ckb-system-scripts

[![Build Status](https://github.com/nervosnetwork/ckb-system-scripts/workflows/CI/badge.svg)](https://github.com/nervosnetwork/ckb-system-scripts/actions)
[![Crates.io](https://img.shields.io/crates/v/ckb-system-scripts)](https://crates.io/crates/ckb-system-scripts)

CKB's system scripts, which included in the system cells in the genesis block.

## Quick Start

```
git submodule init
git submodule update
make install-tools
make all-via-docker
cargo test --all
```

## Release

Tag and publish the release. GitHub Actions will publish the crate.
