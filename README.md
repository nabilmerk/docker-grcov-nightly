![ci](https://github.com/nabilmerk/docker-grcov-nightly/workflows/ci/badge.svg)

# docker-grcov-nightly

Find it on [Docker Hub](https://hub.docker.com/repository/docker/nabilmerk/grcov-nightly).

This image is built with :
- [nightly Rust](https://hub.docker.com/r/rustlang/rust) version,
- [llvm-tools](https://internals.rust-lang.org/t/llvm-tools-a-new-rustup-component-for-binary-inspection-objdump-nm-size-and-profiling-profdata/7830) component,
- [Python3](https://www.python.org/),
- and [lcov-cobertura](https://github.com/eriwen/lcov-to-cobertura-xml) for converting lcov to cobertura format.

The build is done everyday at 23:00 UTC in order to match the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).

Right now, there is only linux/debian/stretch with arch AMD64 that is supported.

Two tags are provided:
- `latest`: build from the last push/release version on the [repository](https://github.com/nabilmerk/docker-grcov-nightly),
- `nightly`: build from scheduled with the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).