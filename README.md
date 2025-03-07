# tmux_conf
A personalized `tmux` configuration for enhanced terminal experience

# Installation & Usage
```bash
# clone the repository
git clone https://github.com/JunyeolYu/tmux_conf.git

# backup your prev .tmux.conf
# mv ~/.tmux.conf ~/.tmux.conf.backup

# link
ln -s tmux_conf/.tmux.conf ~/.tmux.conf
```
## Install Plugins (TPM) (Optional)
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

# Quick Start
You can modify .tmux.conf to fit your workflow.
Some key settings include:
- Default Prefix: `Ctrl + b`
- Reload Configuration:
  - Press `Prefix + r` to reload the `.tmux.conf` file
- Splitting Panes:
  - Vertical: `Prefix + |`
  - Horizontal: `Prefix + -`
- Switching Pane focus:
  - `Alt + Arrow Keys`
- Resizing Panes:
  - `Prefix + h/j/k/l`
- Switching Windows:
  - `Shift + Left/Right`

# Troubleshooting
1. "Unknown command" error in tmux
Possible Causes:
- Line endings issue (CRLF(for Windows) vs. LF)
  On some systems, cloning the repo might result in unwanted CRLF line endings.
  ```bash
  # Check your Git settings
  git config --global core.autocrlf

  # if the result is true,
  git config --global core.autocrlf input
  ```
- Encoding issues
  ```bash
  # Ensure UTF-8 encoding
  file ~/.tmux.conf
  ```
