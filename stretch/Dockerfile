FROM rustlang/rust:nightly-stretch

# Install grcov, llvm-tools (for demangling) and python3 component to convert lcov to cobertura format (useful for Gitlab).
RUN cargo install grcov; \
    rustup component add llvm-tools-preview; \
    apt-get update && apt-get install -yqq python3-pip python3-setuptools lcov; \
    python3 -m pip install wheel; \
    python3 -m pip install lcov_cobertura; \
    rustup --version; \
    cargo --version; \
    rustc --version; \
    grcov --version;