# libcrio 

A library wrapping the crictl

[![libcrio crate](https://img.shields.io/crates/v/libcrio.svg)](https://crates.io/crates/libcrio)
[![libcrio documentation](https://docs.rs/libcrio/badge.svg)](https://docs.rs/libcrio)
[![build status](https://github.com/no9/libcrio/workflows/CI/badge.svg)](https://github.com/no9/libcrio/actions)

With the `libcrio`, developers can programatically access the output of the `crictl` commandline without having to map directly to specific versions of crictl. Useful when you need to support multiple kubernetes flavours.

Used in [IBM Core-Dump-Handler](https://github.com/IBM/core-dump-handler/blob/main/core-dump-composer/) - A core management system for kubernetes.

[Documentation](https://docs.rs/libcrio/)

## Using libcrio

[`libcrio` is available on crates.io](https://crates.io/crates/libcrio).
The recommended way to use it is to add a line into your Cargo.toml such as:

```toml
[dependencies]
libcrio = "2.0.0"
```

Then `use libcrio::Cli;` in your code wherever you want
to call the crictl client. 