![Build and publish Docker image](https://github.com/nabilmerk/docker-grcov-nightly/workflows/Build%20and%20publish%20Docker%20image/badge.svg)
![Scheduled build and publish](https://github.com/nabilmerk/docker-grcov-nightly/workflows/Scheduled%20build%20and%20publish/badge.svg)

# docker-grcov-nightly

Find it on [Docker Hub](https://hub.docker.com/repository/docker/nabilmerk/grcov-nightly).

This image is built with :
- [nightly Rust](https://hub.docker.com/r/rustlang/rust) version,
- [llvm-tools](https://internals.rust-lang.org/t/llvm-tools-a-new-rustup-component-for-binary-inspection-objdump-nm-size-and-profiling-profdata/7830) component,
- [Python3](https://www.python.org/),
- and [lcov-cobertura](https://github.com/eriwen/lcov-to-cobertura-xml) for converting lcov to cobertura format.

The build is done everyday at 23:00 UTC in order to match the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).

Right now, there is only AMD64 that is supported.