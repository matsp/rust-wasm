# rust-wasm

Test project to compile Rust to WebAssembly that can be executed in a standalone runtime like wasmer.

## add rust target

```
rustup target add wasm32-wasi
```

## compile

```
cargo build --release --target wasm32-wasi

--> [242K]  rust-wasm.wasm
```

## execute

```
wasmer rust-wasm.wasm
```
