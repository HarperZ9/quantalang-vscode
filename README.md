# QuantaLang for Visual Studio Code

Syntax highlighting and language support for **[QuantaLang](https://github.com/HarperZ9/quantalang)** - The Effects Language.

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

From the Marketplace: **View → Extensions → search "QuantaLang"**, click Install.

From `.vsix` directly:

```bash
code --install-extension quantalang-0.1.0.vsix
```

## Links

- [Language repo](https://github.com/HarperZ9/quantalang)
- [Grammar repo](https://github.com/HarperZ9/quantalang-tmLanguage)
- [Quanta Universe ecosystem](https://github.com/HarperZ9/quanta-universe)

## License

MIT. Copyright © 2026 Zain Dana Harper.
