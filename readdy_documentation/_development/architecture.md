---
title: Architecture
sectionName: architecture
position: 2
---

### Source tree
```
readdy/
├── README.md
│   ...
│
├── kernels/
│   │
│   ├── cpu/
│   │   ├── include/
│   │   │   └── (kernel includes)
│   │   ├── src/
│   │   │   └── (kernel sources)
│   │   └── test/
│   │       └── (kernel tests)
│   │
│   └── cuda/
│       └── (yet to be added)
│
├── include/
│   └── *.h (core library includes)
│
├── readdy/
│   │
│   ├── main/
│   │   └── (core library sources)
│   └── test/
│       └── (core library tests)
│
├── libraries/
│   └── (pybind11, spdlog)
│
└── wrappers/
    └── python/
        └── src/ (code for python api)
            ├── cxx/
            │   └── (c++ code for the python module)
            │
            └── python/
                └── (python top-level api)

```