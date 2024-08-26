## Helix Configs
These are my personal configuration settings for Elixir development.

### Prerequisites

Before you begin, ensure that you have updated `rustc` to the latest version. You can update Rust using `rustup`:

```bash
rustup update
```

### Language Support

To enhance your development experience in Helix, install the following language servers and tools:
#### Elixir

To install Elixir, use the asdf version manager. Replace <version> with the specific version you need:

```bash
asdf install elixir <version>
```

#### Markdown

For Markdown support in Helix, you will need the following tools:

markdown-oxide: A lightweight Markdown parser and formatter. Install it using Cargo:

```bash
cargo install --locked --git https://github.com/Feel-ix-343/markdown-oxide.git markdown-oxide
```

dprint: A code formatter that supports various languages, including Markdown. Install it using Homebrew:

```bash
brew install dprint
```

### Utilities

These utilities can improve your workflow within the Helix editor:

Tmux: A terminal multiplexer that allows you to run multiple terminal sessions in a single window. Install Tmux via Homebrew:

```bash
brew install tmux
```

LazyGit: A simple terminal UI for Git commands. Install LazyGit using Homebrew:

```bash
brew install lazygit
```

Environment Variables

To ensure all installed tools are accessible from the command line, add the following environment variables to your shell configuration file (e.g., ~/.zshrc or ~/.bashrc):

```bash
# Add local binaries to PATH
export PATH="/usr/local/bin:$PATH"

# Add Elixir language server to PATH
export PATH="$HOME/elixir-ls/release:$PATH"  # Make sure to rename `language_server.sh` to `elixir-ls`
```

After adding these lines, reload your shell configuration:

```bash
source ~/.zshrc  # or source ~/.bashrc
```
