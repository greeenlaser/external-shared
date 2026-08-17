# CGLTF

Version: 1.15

This project was built with [KalaMake](https://github.com/kalakit/kalamake). Use the `.kmake` file with the kalamake CLI to compile [cgltf](https://github.com/jkuhlmann/cgltf) from source.

When compiling this library from scratch:
- Create 'src/cgltf.c' file and fill it with the following data:

```
#define CGLTF_IMPLEMENTATION
#include "cgltf.h"
```
