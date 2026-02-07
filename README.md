# gitpulse

A blazingly fast terminal UI for Git, written in Rust. `gitpulse` aims to provide a smooth, interactive experience for managing Git repositories directly from the terminal.

## Features

- **Fast & responsive** UI built with `ratatui` and `crossterm`.
- **Full Git integration** via the `git2` library.
- **Rich configuration** options via TOML files.
- **Extensible command system** using `clap`.
- **Tracing and logging** with configurable log levels.
- **Cross-platform** support on Windows, macOS, and Linux.

## Installation

```bash

cargo install gitpulse

# Or clone the repository and build from source
git clone https://github.com/Syntax-XXX/gitpulse.git
cd gitpulse
cargo build --release
```

## Usage

```bash
# Show help
gitpulse --help

# Initialize a new repository
gitpulse init

# Add files and commit
gitpulse add .
gitpulse commit -m "Initial commit"

# Push changes
gitpulse push
```

## Configuration

`gitpulse` uses a configuration file (default: `~/.config/gitpulse/config.toml`). Example configuration:

```toml
[log]
level = "info"

[ui]
theme = "dark"
```

## Development

```bash
# Clone the repo
git clone https://github.com/Syntax-XXX/gitpulse.git
cd gitpulse

# Install dependencies
cargo build

# Run the app
cargo run -- .
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

`gitpulse` is licensed under the MIT License. See `LICENSE` for more details.
