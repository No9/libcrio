# libcrio 

A library wrapping the crictl

[![probe crate](https://img.shields.io/crates/v/libcrio.svg)](https://crates.io/crates/libcrio)
[![probe documentation](https://docs.rs/libcrio/badge.svg)](https://docs.rs/libcrio)
[![build status](https://github.com/no9/libcrio/workflows/CI/badge.svg)](https://github.com/no9/libcrio/actions)

With the `probe!` macro, programmers can place static instrumentation
points in their code to mark events of interest. These are compiled into
platform-specific implementations, e.g. SystemTap SDT on Linux. Probes are
designed to have negligible overhead during normal operation, so they can
be present in all builds, and only activated using those external tools.

[Documentation](https://docs.rs/libcrio/)

## Using libcrio

[`libcrio` is available on crates.io](https://crates.io/crates/libcrio).
The recommended way to use it is to add a line into your Cargo.toml such as:

```toml
[dependencies]
libcrio = "0.1"
```

Then `use libcrio::Cli;` in your code wherever you want
to call the crictl client. 