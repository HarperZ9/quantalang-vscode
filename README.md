# QuantaLang for Visual Studio Code

> Syntax highlighting and editor configuration for the QuantaLang effects-oriented systems language.

[![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![vscode](https://img.shields.io/badge/vscode-%5E1.70.0-blue.svg)
![version](https://img.shields.io/badge/version-0.1.0-informational.svg)
[![CI](https://github.com/HarperZ9/quantalang-vscode/actions/workflows/ci.yml/badge.svg)](https://github.com/HarperZ9/quantalang-vscode/actions/workflows/ci.yml)
![deps: none](https://img.shields.io/badge/deps-none-success.svg)
[![part of: Quanta ecosystem](https://img.shields.io/badge/part_of-Quanta_ecosystem-00b3a4.svg)](https://github.com/HarperZ9/quanta-universe)

Syntax highlighting and editor configuration for
**[QuantaLang](https://github.com/HarperZ9/quantalang)**, an effects-oriented
compiler project with a verified C path, shader output, and experimental
backend research.

## Features

- Syntax highlighting for `.quanta` files
- Full keyword coverage - 62 language keywords including the effect system (`with`, `effect`, `handle`, `resume`, `perform`) and AI primitives (`ai`, `neural`, `infer`)
- Smart indentation, bracket matching, and auto-closing pairs
- Comment toggles (`Ctrl+/`)
- File icon for `.quanta`

## About QuantaLang

QuantaLang is an effects-oriented systems language with a multi-backend compiler written in Rust. It compiles to:

- **C** (primary)
- **HLSL**, **GLSL** (shader output)
- **SPIR-V**, **LLVM IR**, **WebAssembly**, **x86-64**, **ARM64**

```quanta
fn main() {
    println!("Hello, World!");
}
```

## Install

From the Marketplace: **View -> Extensions -> search "QuantaLang"**, click Install.

From `.vsix` directly:

```bash
code --install-extension quantalang-0.1.0.vsix
```

## Links

- [Language repo](https://github.com/HarperZ9/quantalang)
- [Grammar repo](https://github.com/HarperZ9/quantalang-tmLanguage)
- [Quanta Universe ecosystem](https://github.com/HarperZ9/quanta-universe)

## License

MIT. Copyright (c) 2026 Zain Dana Harper.
