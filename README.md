![ci](https://github.com/nabilmerk/docker-grcov-nightly/workflows/ci/badge.svg)

# rust-grcov

Find it on [Docker Hub](https://hub.docker.com/repository/docker/nabilmerk/grcov-nightly).

This image is built with :
- [nightly Rust](https://hub.docker.com/r/rustlang/rust) version,
- [llvm-tools](https://internals.rust-lang.org/t/llvm-tools-a-new-rustup-component-for-binary-inspection-objdump-nm-size-and-profiling-profdata/7830) component,
- [Python3](https://www.python.org/),
- and [lcov-cobertura](https://github.com/eriwen/lcov-to-cobertura-xml) for converting lcov to cobertura format.

# Supported architecture

Right now, there is only linux/debian/stretch with arch x86-64 that is supported.

# Supported tags

Signification for tags are provided:
- `latest`: build from the last release version of the [repository](https://github.com/nabilmerk/docker-grcov-nightly),
- `X.Y` or `X.Y.Z`: build from the release `X.Y` or `X.Y.Z` version of the [repository](https://github.com/nabilmerk/docker-grcov-nightly),
- `nightly`: build from scheduled with the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).

The scheduled build (`nightly`) is done everyday at 23:00 UTC in order to match the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).