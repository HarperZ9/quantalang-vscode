# BuildLang for Visual Studio Code

![BuildLang VS Code extension icon](images/icon.png)

> Syntax highlighting and editor configuration for BuildLang `.bld` source files.

[![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![vscode](https://img.shields.io/badge/vscode-%5E1.70.0-blue.svg)
![version](https://img.shields.io/badge/version-0.1.0-informational.svg)
[![CI](https://github.com/HarperZ9/quantalang-vscode/actions/workflows/ci.yml/badge.svg)](https://github.com/HarperZ9/quantalang-vscode/actions/workflows/ci.yml)
![deps: none](https://img.shields.io/badge/deps-none-success.svg)
[![part of: BuildLang ecosystem](https://img.shields.io/badge/part_of-BuildLang_ecosystem-00b3a4.svg)](https://harperz9.github.io/buildlang.html)

Syntax highlighting and editor configuration for
**BuildLang**, an effects-oriented compiler project with the `buildc` CLI, `.bld`
source files, a verified C path, shader output, and experimental backend
research.

## Current status

This branch is the BuildLang VS Code packaging surface for `.bld` files. The VS
Code language id remains `buildlang`, the compiler binary is `buildc`, and the
repository still uses its legacy GitHub slug until the public repo rename is
finished.

## Features

- Syntax highlighting for `.bld` files
- Full keyword coverage - 61 language keywords including the effect system (`with`, `effect`, `handle`, `resume`, `perform`) and AI primitives (`ai`, `neural`, `infer`)
- Smart indentation, bracket matching, and auto-closing pairs
- Comment toggles (`Ctrl+/`)
- File icon for `.bld`

## About BuildLang

BuildLang is an effects-oriented systems language with a multi-backend compiler written in Rust. It compiles to:

- **C** (primary)
- **HLSL**, **GLSL** (shader output)
- **SPIR-V**, **LLVM IR**, **WebAssembly**, **x86-64**, **ARM64**

```text
fn main() ~ Console {
    println!("Hello from BuildLang!");
}
```

## Install

From the Marketplace: **View -> Extensions -> search "BuildLang"**, click Install.

From `.vsix` directly:

```bash
code --install-extension buildlang-0.1.0.vsix
```

## Usage

Once installed, the extension activates automatically for any file with the
`.bld` extension - no commands or configuration required. See
**[USAGE.md](USAGE.md)** for what the extension provides, how to verify it is
active, and worked examples (including a sample under
[`examples/`](examples/)).

This extension is editor support only; it provides syntax highlighting and
language configuration. It does not bundle or run the BuildLang compiler. To
build or run `.bld` programs, use the `buildc` toolchain from the
[BuildLang compiler repo](https://github.com/HarperZ9/quantalang).

## Links

- [BuildLang compiler repo](https://github.com/HarperZ9/quantalang)
- [BuildLang TextMate grammar](https://github.com/HarperZ9/quantalang-tmLanguage)
- [Build ecosystem repository](https://github.com/HarperZ9/quanta-universe)

## Development

For developers:

Validate the public extension surface before pushing:

```bash
python -m json.tool package.json
python -m json.tool language-configuration.json
python -m json.tool syntaxes/buildlang.tmLanguage.json
npm pack --dry-run
```

Quick local check:

```bash
npm pack --dry-run
```

## License

MIT. Copyright (c) 2026 Zain Dana Harper.
