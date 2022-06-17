# ckb-system-scripts

[![Build Status](https://github.com/nervosnetwork/ckb-system-scripts/workflows/CI/badge.svg)](https://github.com/nervosnetwork/ckb-system-scripts/actions)
[![Crates.io](https://img.shields.io/crates/v/ckb-system-scripts)](https://crates.io/crates/ckb-system-scripts)

CKB's system scripts, which included in the system cells in the genesis block.

We create a new lock script called `secp256k1_blake160_sighash_all-sub` lock which is different from the offical `secp256k1_blake160_sighash_all` lock as follows:

1. Change the `MAX_WITNESS_SIZE` from 32768 to 327680 (320k bytes)
2. The size of lock args must be greater than or equal to 20bytes and less than or equal to 64bytes

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
