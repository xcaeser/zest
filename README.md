# zest 🍋

<div>

**zest** is an experimental, source-based package manager built in [Zig](https://ziglang.org).  
It draws inspiration from [Homebrew](https://brew.sh), aiming for simplicity, clarity, and performance.

[![Version](https://img.shields.io/badge/Zig_Version-0.14.0-orange.svg?logo=zig)](README.md)
[![MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg?logo=cachet)](LICENSE)
[![Version](https://img.shields.io/badge/zest-v0.0.1%20alpha-green)](https://github.com/xcaeser/zest/releases)

</div>

> [!IMPORTANT]
> **This project is in exploration phase.**
> APIs, structure, and behavior may change significantly.
> Not production-ready. Use at your own risk.

## ✨ Goals

- Lightweight CLI package manager
- Git-based formula repository
- Source builds with verified downloads
- Written 100% in Zig

## 🚀 Example (planned)

```sh
zest install curl
zest update
zest list
```

## 📁 Formula Format (WIP)

Formulas are defined as `.zig` files:

```zig
pub const formula = struct {
    pub const name = "curl";
    pub const version = "8.7.1";
    pub const url = "https://curl.se/download/curl-8.7.1.tar.gz";
    pub const sha256 = "abc123...";
    pub fn install() !void {
        // Installation logic goes here
    }
};
```

## 📦 License

MIT
