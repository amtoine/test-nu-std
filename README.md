# a draft demo of what a modular standard library **could** be

## the files
```bash
.
└── standard_library
    ├── assert
    │   ├── mod.nu
    │   └── tests.nu
    ├── dirs
    │   ├── mod.nu
    │   └── tests.nu
    ├── std.nu
    └── tests.nu

4 directories, 6 files
```

we can assume the root of this repo is a mock-up of the current `crates/nu-utils/` of `nushell` :thumbsup:

## use the library
```bash
>_ use standard_library/std.nu
>_ help std
Module: std

Exported commands:
  assert (std assert), assert eq (std assert eq), assert ne (std assert ne), dirs add (std dirs add), dirs show (std dirs show)

This module does not export environment.
```

## run the tests
```bash
>_ nu tests.nu
tests for assert
tests for dirs
```
