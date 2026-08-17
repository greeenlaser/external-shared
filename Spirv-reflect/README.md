# spir-v-reflect

Version: 1.4.357.0

This project was built with [KalaMake](https://github.com/kalakit/kalamake). Use the `.kmake` file with the kalamake CLI to compile [spirv-reflect](https://github.com/KhronosGroup/SPIRV-Reflect) from source.

When compiling this library from scratch:
- Copy `spirv_reflect.c` to `src` and `spirv_reflect.h` to `include`
- Go into `include/spirv_reflect.h` and change `#include "./include/spirv/unified1/spirv.h"` to `#include "spirv/unified1/spirv.h"`
