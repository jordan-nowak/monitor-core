# monitor-core
monitor-core is a modular C++ library designed for robotics and real-time systems, providing structured multi-level logging (console and file), metadata management, monitoring utilities, and chrono helpers with a clean and extensible architecture.

---

## Modules Description

### logging
- Log levels (Trace, Debug, Info, Warning, Error)
- Console and file outputs
- Configurable verbosity at runtime

### monitoring
- Runtime metrics collection
- Performance tracking utilities

### chrono
- Execution time measurement utilities

---

## Installation And Usage Instructions

Clone the source code locally:
    ```bash
    git clone https://github.com/jordan-nowak/monitor-core.git
    cd monitor-core
    mkdir build && cd build
    cmake ..
    cmake --build .
    ```

Configure the compiler and build the library to obtain executable:
    ```bash
    cd monitor-core/build
    cmake -G Ninja -DCMAKE_BUILD_TYPE=Release ..
    cmake --build .
    ```
    Or just `ninja` command to build following your environment.

Tested with:
- GCC 15.2.0 (MSYS2)
- CMake 4.2.1
- Ninja 1.13.2

---

## Development Contribution
If you develop, please create a new branch ('feature', 'chore', 'fix', 'doc', 'test'...) on the 'develop' branch, following these steps:
```bash
git checkout develop
git pull origin develop
git checkout -b feature/xxxx-SimpleTitleToDescribeTheFeature
```

Nb: `xxxx` represents the incremental feature number.

---
## Run Tests

Don't forget to develop tests for each development made. It is necessary to add them to CMakeList.txt and run all tests with the following command: 
```bash
ctest
```

It is possible to add arguments after the execution command to obtain more details:
```bash
ctest --verbose
```

Or prevent execution from continuing if there is a failure:
```bash
ctest --output-on-failure
```

---

## Versioning

monitor-core follows _Semantic Versioning_:

MAJOR.MINOR.PATCH
- MAJOR: Breaking changes
- MINOR: New features (backward compatible)
- PATCH: Bug fixes

---

### [WORK IN PROGRESS] Offline API Documentation

With [Doxygen](https://www.doxygen.nl) installed, the documentation can be built locally by...

The resulting documentation can be accessed by opening `monitor-core/docs/html/index.html` in a web browser.

---

## License

The license that applies to the whole package content is MIT. Please look at the [LICENSE](./LICENSE) file at the root of this repository for more details.

---

## Maintainer

- Jordan NOWAK (JNo)