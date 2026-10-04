# Third-Party Licenses

LightningCSV incorporates the third-party open-source software listed below. Each component is used under its own license.

LightningCSV itself is proprietary software (see `LICENSE.md`). The licenses below apply only to the respective components.

## Runtime Environment (not bundled)

### Microsoft Edge WebView2 Runtime (Windows)
- Windows builds render the UI with the WebView2 Runtime installed on the system (preinstalled on Windows 11). It is not bundled with this application.
- **License**: Subject to the [Microsoft Edge WebView2 Runtime license terms](https://developer.microsoft.com/microsoft-edge/webview2/), not this project's license

### WebKit / WKWebView (macOS)
- macOS builds render the UI with the system WKWebView, which is part of macOS and is not bundled with this application.

## Application Framework

### Tauri v2
- **License**: MIT OR Apache-2.0
- **Copyright**: Tauri Programme within The Commons Conservancy
- **URL**: https://github.com/tauri-apps/tauri
- Includes wry (MIT OR Apache-2.0) and tao (Apache-2.0)
- Plugins used: tauri-plugin-dialog, tauri-plugin-shell, tauri-plugin-log, tauri-plugin-single-instance (each MIT OR Apache-2.0)

## Rust Backend Dependencies

- **duckdb (duckdb-rs) / libduckdb-sys / DuckDB**: MIT License - Stichting DuckDB Foundation / duckdb-rs contributors (SQL search, sort, Parquet output)
  - DuckDB itself bundles third-party components under their own permissive licenses; see https://github.com/duckdb/duckdb (`LICENSE` and `third_party/`).
- **memmap2**: MIT OR Apache-2.0
- **csv / csv-core**: Unlicense OR MIT - Andrew Gallant
- **encoding_rs**: (Apache-2.0 OR MIT) AND BSD-3-Clause - Mozilla Foundation (BSD-3-Clause applies to data from the WHATWG Encoding Standard)
- **chardetng**: Apache-2.0 OR MIT - Mozilla Foundation
- **regex**: MIT OR Apache-2.0 - The Rust Project Developers
- **rayon**: MIT OR Apache-2.0
- **serde / serde_json**: MIT OR Apache-2.0
- **log**: MIT OR Apache-2.0
- **anyhow / thiserror**: MIT OR Apache-2.0 - David Tolnay
- **toml**: MIT OR Apache-2.0
- **dirs-next**: MIT OR Apache-2.0
- **windows-sys** (Windows only): MIT OR Apache-2.0 - Microsoft Corporation
- **core-foundation** (macOS only): MIT OR Apache-2.0 - The Servo Project Developers
- **objc2** (macOS only): MIT - Mads Marquart
- Transitive dependencies (see `src-tauri/Cargo.lock`) are under the following licenses:
  MIT, Apache-2.0, BSD-3-Clause, Zlib, Unicode-3.0, CC0-1.0, Unlicense, BSL-1.0 (each where it is the license or one of the license options),
  and **MPL-2.0** (cssparser, cssparser-macros, dtoa-short, selectors via Tauri; option-ext via dirs-next; all used unmodified)

## Frontend Dependencies

- **react / react-dom / scheduler**: MIT License - Meta Platforms, Inc. and affiliates
- **zustand**: MIT License - Paul Henschel
- **i18next / react-i18next**: MIT License - i18next contributors
  (includes @babel/runtime, html-parse-stringify, void-elements: MIT)
- **lucide-react**: ISC License - Lucide Contributors (portions MIT, Cole Bemis / Feather)
- **@tauri-apps/api, @tauri-apps/plugin-dialog, @tauri-apps/plugin-shell**: MIT OR Apache-2.0

---

## License Compatibility

This project is distributed under a proprietary license (see `LICENSE.md`). All third-party components listed above are licensed under open-source licenses that permit their inclusion in proprietary, closed-source, and commercially distributed software, provided the required copyright and license notices are retained (as listed in this document):

- **MIT / BSD-2-Clause / BSD-3-Clause / ISC / Zlib / Unlicense / CC0-1.0 / BSL-1.0 / Unicode-3.0**: Permissive, no copyleft or source-disclosure obligations
- **Apache License 2.0**: Permissive, requires preservation of copyright and license notices
- **Mozilla Public License 2.0** (cssparser, selectors, etc.): File-level copyleft; applies only to those libraries' own source files, which are used unmodified. The source code of these libraries is available from https://crates.io and their repositories. It does not extend to this application's code.

No GPL / LGPL / AGPL-only dependencies are included.

## Full License Texts

For complete license texts of each library, please refer to their respective repositories or package registries:

- Rust crate licenses: see each crate's repository or https://crates.io (crate names and versions are listed in `src-tauri/Cargo.lock`)
- Frontend library licenses: see each package on https://www.npmjs.com (versions are listed in `package-lock.json`)
- Apache License 2.0: https://www.apache.org/licenses/LICENSE-2.0
- Mozilla Public License 2.0: https://www.mozilla.org/MPL/2.0/
