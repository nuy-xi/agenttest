# agenttest

A small C++ sandbox repository.

## Layout

| Path | Purpose |
| --- | --- |
| `hello-cpp/` | Minimal C++17 program |

## Build and run

Requires CMake 3.20 or newer and a C++17 compiler.

```sh
cmake -S hello-cpp -B build
cmake --build build
ctest --test-dir build --output-on-failure
./build/hello
```

The build directory is already covered by `.gitignore`.
