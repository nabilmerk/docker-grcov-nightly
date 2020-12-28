![ci](https://github.com/nabilmerk/docker-grcov-nightly/workflows/ci/badge.svg)

# rust-grcov

Find it on [Docker Hub](https://hub.docker.com/repository/docker/nabilmerk/grcov-nightly).

This image is built with :
- [nightly Rust](https://hub.docker.com/r/rustlang/rust) version,
- [grcov](https://github.com/mozilla/grcov) tool,
- [llvm-tools](https://internals.rust-lang.org/t/llvm-tools-a-new-rustup-component-for-binary-inspection-objdump-nm-size-and-profiling-profdata/7830) component,
- [Python3](https://www.python.org/) runner,
- and [lcov-cobertura](https://github.com/eriwen/lcov-to-cobertura-xml) tool for converting lcov to cobertura format.

# Supported architecture

Right now, there is only linux/debian/stretch with arch x86-64 that is supported.

| Architecture                      | Supported        | Comments            |
| --------------------------------- |:----------------:| ------------------- |
| Linux x86-64 (`amd64`)            |:heavy_check_mark:| Debian Stretch only |
| ARMv6 32-bit (`arm32v6`)          |:x:               |                     |
| ARMv7 32-bit (`arm32v7`)          |:x:               |                     |
| ARMv8 64-bit (`arm64v8`)          |:x:               |                     |
| Windows x86-64 (`windows-amd64`)  |:x:               |                     |

# Supported tags

Signification for tags are provided:
- `latest`: build from the last release version of the [repository](https://github.com/nabilmerk/docker-grcov-nightly),
- `X.Y` or `X.Y.Z`: build from the release `X.Y` or `X.Y.Z` version of the [repository](https://github.com/nabilmerk/docker-grcov-nightly),
- `nightly` or `YYYYMMDD`: build from scheduled with the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).

The table hereafter defines how components are updated:
| Tag | Rust | grcov | llvm-tools | Python3 | lcov-cobertura |
-|||||||-
| `latest` <td colspan=5> building date of rust-grcov latest release (rust version is the nightly Rust of the building date)
| `X.Y` or `X.Y.Z` <td colspan=5> building date of rust-grcov `X.Y` or `X.Y.Z` release (rust version is the nightly Rust of the building date)
| `nightly` or `YYYYMMDD` | nightly <td colspan=4> last release


The scheduled build (`nightly`) is done everyday at 23:00 UTC in order to match the last release of [nightly Rust](https://hub.docker.com/r/rustlang/rust).