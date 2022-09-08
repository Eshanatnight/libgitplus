# libgit2cpp

[![AppVeryor Build Status](https://ci.appveyor.com/api/projects/status/ps6e0s4nfnw5afh4/branch/master?svg=true)](https://ci.appveyor.com/project/AndreyG/libgit2cpp/branch/master)

C++ wrapper for libgit2. It contains libgit2 as submodule (libs/libgit2).

## Building libgit2cpp - Using CMake

```bash
    mkdir build
    cd build
    cmake ..
    cmake --build .
```

### CMake Options

Supporting CMake options:

* `USE_BOOST`
* `BUNDLE_LIBGIT2`
* `BUILD_LIBGIT2CPP_EXAMPLES`

## Testing

```bash
cd build
./test.sh <path_to_non_shared_repo> [path_to_libgit2_testrepo]
```

### Example

```bash
mkdir build && cd build
cmake ..
make
./test.sh .. ../libs/libgit2/tests/resources/testrepo.git
```
