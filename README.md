# a draft demo of what a modular standard library **could** be

## the files
```bash
.
├── assert
│   ├── mod.nu
│   └── tests.nu
├── dirs
│   ├── mod.nu
│   └── tests.nu
├── LICENSE
├── std.nu
└── tests.nu

3 directories, 7 files
```

## use the library
```bash
>_ use std.nu
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
