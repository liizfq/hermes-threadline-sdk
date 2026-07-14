# Hermes Threadline SDK

Standalone Android library module containing the generated Kotlin bindings and arm64-v8a native library used by [Hermes Threadline](https://github.com/liizfq/hermes-threadline).

This repository is derived from the [matrix-rust-sdk](https://github.com/matrix-org/matrix-rust-sdk) Android FFI output. The generated bindings and native library are kept separate from the Android client so they can be versioned and rebuilt independently.

## Contents

- Generated Kotlin UniFFI bindings
- `libmatrix_sdk_ffi.so` for `arm64-v8a`
- Gradle Android library module configuration

## Usage

Include this repository as the `:sdk-local` module in the Hermes Threadline checkout. The client expects the module path to remain `sdk-local`.

## ABI

Only `arm64-v8a` is currently included.

## Rebuilding

Regenerate the bindings and native library from the corresponding matrix-rust-sdk checkout, then replace the generated Kotlin files and native library in this repository.
