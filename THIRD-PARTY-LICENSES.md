# Third-Party Licenses

This software uses the following third-party libraries and their respective licenses:

## Application Runtime

### Tauri v2
- **License**: MIT License / Apache License 2.0 (dual)
- **Copyright**: Tauri Programme within The Commons Conservancy
- **URL**: https://github.com/tauri-apps/tauri
- Plugins used: tauri-plugin-dialog, tauri-plugin-fs, tauri-plugin-shell, tauri-plugin-updater, tauri-plugin-log, tauri-plugin-single-instance (each MIT OR Apache-2.0)

### Microsoft Edge WebView2 Runtime (Windows)
- Windows builds render the UI using the WebView2 Runtime, which is provided by Microsoft and is not bundled inside this application.
- **License**: Subject to the [Microsoft Edge WebView2 Runtime license terms](https://developer.microsoft.com/microsoft-edge/webview2/), not this project's license
- **URL**: https://developer.microsoft.com/microsoft-edge/webview2/

## Rust Backend Dependencies

- **duckdb (duckdb-rs) / DuckDB**: MIT License - DuckDB Foundation / DuckDB contributors (SQL search, sort, Parquet output)
- **memmap2**: MIT OR Apache-2.0
- **csv / csv-core**: Unlicense OR MIT - Andrew Gallant
- **encoding_rs**: (Apache-2.0 OR MIT) AND BSD-3-Clause - Mozilla Foundation
- **chardetng**: Apache-2.0 OR MIT - Mozilla Foundation
- **regex**: MIT OR Apache-2.0
- **rayon**: MIT OR Apache-2.0
- **serde / serde_json**: MIT OR Apache-2.0
- **log**: MIT OR Apache-2.0
- **anyhow / thiserror**: MIT OR Apache-2.0
- **toml**: MIT OR Apache-2.0
- **dirs-next**: MIT OR Apache-2.0
- **windows-sys**: MIT OR Apache-2.0 - Microsoft Corporation
- Transitive dependencies (see `src-tauri/Cargo.lock`) are under the following licenses:
  MIT, Apache-2.0, BSD-2-Clause, BSD-3-Clause, ISC, Zlib, Unlicense, CC0-1.0, Unicode-3.0, CDLA-Permissive-2.0,
  and **MPL-2.0** (cssparser, cssparser-macros, dtoa-short, option-ext, selectors; used unmodified via Tauri and dirs-next)

## Frontend Dependencies

- **react / react-dom**: MIT License - Meta Platforms, Inc. and affiliates
- **zustand**: MIT License - Paul Henschel, Daishi Kato
- **i18next / react-i18next**: MIT License - i18next contributors
- **lucide-react**: ISC License - Lucide Contributors (portions MIT, Cariet Corp / Feather)
- **@tauri-apps/api and plugins (dialog, fs, shell, updater)**: MIT OR Apache-2.0

---

## License Compatibility

This project is distributed under a proprietary license (see `LICENSE.md`). All third-party components listed above are licensed under open-source licenses that permit their inclusion in proprietary, closed-source, and commercially distributed software, provided the required copyright and license notices are retained (as listed in this document):

- **MIT / BSD 2-Clause / BSD 3-Clause / ISC / Zlib / Unlicense / CC0**: Permissive, no copyleft or source-disclosure obligations
- **Apache License 2.0**: Permissive, requires preservation of copyright and license notices
- **Mozilla Public License 2.0** (cssparser, selectors, etc.): File-level copyleft; applies only to those libraries' own source files, which are used unmodified. It does not extend to this application's code.

No GPL / LGPL / AGPL-only dependencies are included.

## Full License Texts

For complete license texts of each library, please refer to their respective repositories or package registries:

- Rust crate licenses: see each crate's repository (crate names and versions are listed in `src-tauri/Cargo.lock`)
- Frontend library licenses: see `node_modules/<package>/LICENSE` or run `npm info [package-name] license`
