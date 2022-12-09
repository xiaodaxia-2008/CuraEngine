# Building Notes

- C++20 is used.
- Using `vcpkg` to install dependencies.

```shell
vcpkg install polyclipping stb rapidjson spdlog range-v3
```

- Disable arcus: `-DENABLE_ARCUS=OFF`

- Run 
```shell
cmake .. --toolchain /path/to/vcpkg.cmake --config Debug
cmake --build . --config Debug
```