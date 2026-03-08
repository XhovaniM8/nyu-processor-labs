# NYU Processor Design - Onboarding Labs

Onboarding labs for the NYU Processor Design team. Covers the toolchain and workflow used in the project.

## Stack

- **HDL:** SystemVerilog
- **Simulation:** Verilator
- **Testing:** Catch2 (C++)
- **Build:** CMake + Ninja
- **Packages:** vcpkg

## Labs

| Lab | Topic |
|-----|-------|
| [lab-1](labs/lab-1) | CMake basics and toolchain setup |
| [lab-2](labs/lab-2) | SystemVerilog modules and C++ testbenches |
| [lab-3](labs/lab-3) | Verification strategies (exhaustive, sampling, random) |
| [lab-4](labs/lab-4) | Package management with vcpkg |
| [lab-5](labs/lab-5) | Full project template with CI/CD |
| [lab-6](labs/lab-6) | See lab-7 |
| [lab-7](labs/lab-7) | Processor design notes |
| [lab-8](labs/lab-8) | TBD |

## Building (labs 2-5)

```sh
cmake -S . -B build -G Ninja
cmake --build build
ctest --test-dir build
```

Dependencies are managed via vcpkg and bootstrapped automatically by CMake.
