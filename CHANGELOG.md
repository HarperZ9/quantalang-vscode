# Changelog

## Unreleased

- Refreshes the public presentation as the BuildLang VS Code package for
  `.bld` files and the `buildc` toolchain.
- Updates CI and release workflows to current first-party GitHub Actions
  majors.
- Adds GitHub funding metadata and a README developer verification section.

## 0.1.0 - 2026-04-12

Initial release.

- Syntax highlighting for `.bld` files based on the official TextMate grammar
- Language configuration for brackets, comments, and auto-closing pairs
- 61 recognized keywords, including effect-system and AI primitive keywords
- Primitive type highlighting from `i8` through `u128`, plus floating-point,
  boolean, character, string, and common standard-library types
- Lifetime, macro, and attribute highlighting
- String interpolation inside quoted strings
