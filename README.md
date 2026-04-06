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

Search session transcripts for a remembered topic:

```command
claude-history --search serde
```

When several sessions match, `claude-history` will prompt you to choose one in an interactive terminal. You can also combine search with `--list` to show matching sessions without opening a transcript:

```command
claude-history --search "rust serialization library" --list
```

For release and repository workflow details, see `CONTRIBUTING.md`.

For example:

```command
claude-history --workspace /path/to/workspace
```

```command
claude-history -w
```
