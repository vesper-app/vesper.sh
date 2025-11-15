<div align="center">

![Vesper Logo](./assets/logo.png)
<!-- This is a placeholder path. Replace with your actual logo file. -->

# Vesper.sh
### Your persistent, predictable, terminal workspace.

[![Build Status](https://img.shields.io/github/actions/workflow/status/vesper-app/vesper/build.yml?branch=main&style=for-the-badge)](https://github.com/vesper-app/vesper/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Latest Release](https://img.shields.io/github/v/release/vesper-app/vesper?style=for-the-badge)](https://github.com/vesper-app/vesper/releases)

Tired of fighting your terminal multiplexer? Vesper is a modern, standalone alternative to Tmux that works out of the box.

**[Visit Vesper.sh for full documentation & guides](https://vesper.sh)**

</div>

---

## 🚀 Installation

Vesper is a standalone application. Ensure you have **Neovim (v0.8+)** installed on your system.

### macOS / Homebrew
```bash
brew install vesper
```

### Arch Linux / AUR
Use your preferred AUR helper (e.g., `yay` or `paru`):
```bash
yay -S vesper
```

### Build from source (universal Linux)
Requires the Rust toolchain (`cargo`).
```bash
git clone https://github.com/vesper-app/vesper.git
cd vesper
cargo install --path .
```

## ✨ Why Vesper?

### Rock-solid persistence: never lose your work
We've all been there: your SSH connection drops and your work vanishes. Vesper was built to solve this. When you detach—on purpose or by accident—your entire session is safe. Re-attaching is instant, putting you right back where you left off.

### Fluid rendering, no glitches
Vesper uses the core rendering engine from Neovim. This means you get a terminal experience that's incredibly fast, with zero screen-tearing or graphical glitches. It handles true-color and Unicode perfectly.

### Intuitive window management
No more fighting with prefix keys and confusing commands. Vesper's pane management is simple and predictable. Splitting, resizing, and navigating windows feels natural and is designed to stay out of your way.

## ⚡ Quickstart guide

Get started in less than a minute.

1.  **Launch Vesper:**
    ```bash
    vesper
    ```
2.  **Use these essential commands:**

| Action | Keybinding | Description |
| :--- | :--- | :--- |
| **Split pane vertically** | `Ctrl-v` | Divides the current pane side-by-side. |
| **Split pane horizontally**| `Ctrl-h` | Divides the current pane top-and-bottom. |
| **Navigate panes** | `Alt` + `h/j/k/l` | Moves focus between panes (Vim-style). |
| **Detach session** | `Ctrl-d` | Archives the session and returns to your shell. |
| **Re-attach session** | `vesper attach` | Restores the last active session. |


### Managing multiple sessions

- **Start a new, named session:**
  ```bash
  vesper new -s my-project-name
  ```
- **List all active sessions:**
  ```bash
  vesper list
  ```
- **Attach to a specific session:**
  ```bash
  vesper attach -s my-project-name
  ```

---

## 🤝 Contributing

Contributions are welcome! Vesper is built by and for its community. Whether it's bug reports, feature requests, or pull requests, we'd love to have your help.

Check out our **[Contributing Guide](https://github.com/vesper-app/vesper/blob/main/CONTRIBUTING.md)** to get started, and join our **[Discord Server](https://your-discord-link)** to connect with other developers.

## 📄 License

Vesper is open-source software licensed under the [MIT License](https://opensource.org/licenses/MIT).
```