# Claude History

Get a transcript of your last Claude Code session, ready to include in your commit message.

## Installation

With Homebrew:

```command
brew install simonwhitaker/tap/claude-history
```

With Cargo:

```command
cargo install claude-code-history
```

For local development, use `cargo install --path .`.

Then run `claude-history` from the same directory where you previously ran `claude`, pass `--workspace /path/to/workspace` to target a different workspace, or pass `-w` to choose from available workspaces interactively.

## Usage

To get a list of command-line options:

```command
claude-history --help
```

For release and repository workflow details, see `CONTRIBUTING.md`.

For example:

```command
claude-history --workspace /path/to/workspace
```

```command
claude-history -w
```
