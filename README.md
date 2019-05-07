## runtime example module:
A simple example of a runtime module demonstrating
concepts, APIs and structures common to most runtime modules.

This repo serves as a template for writing new modules for substrate runtimes
as independent reusable rust library.

The main `lib.rs` also has a template for writing documentation for the module, following the same style as substrate srml modules. This can be easily derived from the specs written for the module during the design phase.

Since there isn't yet a stable substrate release we are still using a commit hash when referencing the dependencies on substrate packages in Cargo.toml. The same commit hash should be used in the runtime library.
Eventually when a stable API is reached we can move to using version numbers and get dependencies from published crates on crates.io

Consuming the module in a substrate runtime:
Here is a [sample PR](https://github.com/joystream/substrate-runtime-joystream/) for how to use the module in the Joystream runtime.

Rust docs can be viewed by running:

`cargo doc --package runtime-example-module --open`

Recommended style guides:

Joystream Rust : https://github.com/Joystream/joystream/issues/36

Substrate Rust: https://wiki.parity.io/Substrate-Style-Guide
