# bevy-wasm-test
Follows the [Bevy Cheatbook wasm section](https://bevy-cheatbook.github.io/platforms/wasm.html).

# Dependencies
Required to run locally.

```
rustup target install wasm32-unknown-unknown
cargo install wasm-server-runner
```

# Building
Generate game files for a webserver.

```
cargo build --release --target wasm32-unknown-unknown
wasm-bindgen --out-dir ./out/ --target web ./target/
```
