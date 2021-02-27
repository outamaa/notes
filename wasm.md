---
date: 2021-02-27
---

# WebAssembly

## Rust, SDL2, OpenGL, Wasm

Check out [rust_sdl2_opengl_emscripten](https://github.com/therocode/rust_sdl2_opengl_emscripten) repo. Some things to keep in mind:

### Emscripten version

At the time of writing, due to LLVM related compatibility stuff, Rust projects build
with Emscripten version 1.39.20. To use this specific version:

```shell
git clone https://github.com/emscripten-core/emsdk.git
cd emsdk
./emsdk install 1.39.20
./emsdk activate 1.39.20
source ./emsdk_env.sh
```
