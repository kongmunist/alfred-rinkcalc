# Rinkcalc — Alfred workflow

Unit-aware scientific calculator for Alfred, powered by [rink](https://rinkcalc.app).

Type `r ` followed by an expression: `r 3V*3V*100uF`, `r 60 mph to m/s`, `r sqrt(2)`, `r speed of light`, `r 1 GB to MiB`. Hit return to copy the result.

## Install

The bundled `rink` binary is `aarch64-apple-darwin` (Apple Silicon).

1. Open `Rinkcalc.alfredworkflow` in Finder (or zip the contents of this repo and rename the zip to `.alfredworkflow`), then double-click to import into Alfred.
2. Or copy this directory into `~/Library/Application Support/Alfred/Alfred.alfredpreferences/workflows/<any-uuid>/` and restart Alfred.

The script resolves `rink` in this order: bundled binary next to `info.plist` → `rink` on `$PATH` → `~/.cargo/bin/rink`. Intel users (or anyone who'd rather not run the bundled binary) can `cargo install rink` and delete the bundled copy.

## Credits

- [rink](https://github.com/tiffany352/rink-rs) by Tiffany Bennett — MPL-2.0 / GPL-3.0-or-later. Source: https://github.com/tiffany352/rink-rs
