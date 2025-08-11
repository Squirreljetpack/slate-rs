# slate-rs [![Crates.io](https://img.shields.io/crates/v/slate-rs)](https://crates.io/crates/slate-rs)[![License](https://img.shields.io/github/license/squirreljetpack/slate-rs)](https://github.com/squirreljetpack/slate-rs/blob/main/LICENSE)

Fork of https://github.com/znx3p0/vielsprachig, with extra functionality


# Installation

```shell
cargo install slate-rs

# Convert yml -> toml
slate $HOME/.config/alacritty.yml -o $HOME/.config/alacritty.toml
```

# Features
- Convert between different input and output serialized data formats
- Tera templating
- Special modes for generating systemd timers and quadlet files (see examples)

## Supported formats
The current input options and their inferred extensions are:

| Input | Output       | Extensions               |
|-------|--------------|--------------------------|
| Json  | Json         | `.json`                  |
|       | PrettyJson   | `.hjson`                 |
| Yaml  | Yaml         | `.yaml`, `.yml`          |
| Cbor  | Cbor         | `.cb`, `.cbor`           |
| Ron   | Ron          | `.ron`                   |
|       | PrettyRon    | `.hron`                  |
| Toml  | Toml         | `.toml`                  |
| Bson  | Bson         | `.bson`, `.bs`           |
|       | Pickle       | `.pickle`, `.pkl`        |
|       | Bincode      | `.bc`, `.bincode`        |
|       | Postcard     | `.pc`, `.postcard`       |
|       | Flexbuffers  | `.fb`, `.flexbuffers`    |
|       | Systemd      | (use `--to systemd`)     |
|       | Quadlet      | (use `--to quadlet`)     |


# See also

- https://matduggan.com/replace-compose-with-quadlet/

- https://chasingsunlight.netlify.app/posts/homelab-with-docker-and-tailscale-2/