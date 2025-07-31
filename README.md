# My Tmux Configuration

This repository contains my personal tmux configuration. It's designed for a highly efficient, keyboard-driven workflow, with a focus on simplicity and ease of use.

## Features

*   **Plugin Management:** Uses `tpm` (Tmux Plugin Manager) for easy management of tmux plugins.
*   **Custom Keybindings:** A set of intuitive keybindings for session, window, and pane management.
*   **Theming:** A clean and modern theme using `tmux2k` with the `catppuccin` theme.
*   **Seamless Navigation:** Easy navigation between windows and panes.
*   **Clipboard Integration:** Uses `tmux-yank` for easy copying to the system clipboard.
*   **Session Persistence:** `tmux-resurrect` and `tmux-continuum` for saving and restoring tmux sessions.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/your-repo-name.git ~/.config/tmux
    ```

2.  **Install `tpm`:**

    ```bash
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```

3.  **Install the plugins:**

    *   Start tmux.
    *   Press `prefix` + `I` (that's a capital I) to fetch the plugins.

## Keybindings

### Session Management

| Key         | Description                  |
| ----------- | ---------------------------- |
| `Ctrl-c`    | Create a new session         |
| `r`         | Reload the tmux configuration|

### Window Management

| Key         | Description                  |
| ----------- | ---------------------------- |
| `Alt-o`     | Create a new window          |
| `Alt-O`     | Break a pane into a new window|
| `Alt-Q`     | Kill the current pane        |
| `Ctrl-p`    | Go to the previous window    |
| `Ctrl-n`    | Go to the next window        |
| `Alt-1`...`9`| Select window 1 through 9    |
| `N`         | Rename the current window    |
| `W`         | Choose a window from a list  |
| `E`         | Swap the current window with another |

### Pane Management

| Key         | Description                  |
| ----------- | ---------------------------- |
| `|`         | Split the window horizontally|
| `-`         | Split the window vertically  |
| `Alt-h/j/k/l`| Navigate between panes       |
| `Alt-H/J/K/L`| Resize panes                 |
| `Alt-f`     | Toggle pane zoom             |
| `>`         | Swap pane with the next one  |
| `<`         | Swap pane with the previous one|
| `Alt-Space` | Cycle through pane layouts   |
| `1`...`9`    | Select pane 1 through 9      |

### Copy Mode (Vi-style)

| Key         | Description                  |
| ----------- | ---------------------------- |
| `Alt-v`     | Enter copy mode              |
| `v`         | Begin selection              |
| `y`         | Copy selection               |
| `Y`         | Copy to the end of the line  |

### Other

| Key         | Description                  |
| ----------- | ---------------------------- |
| `Ctrl-q`    | Clear screen and history     |
| `T`         | Toggle synchronize-panes     |

## Theming

The theme is provided by the `tmux2k` plugin, using the `catppuccin` theme. The status bar is configured to show:

*   **Left:** Session name, CPU usage, and RAM usage.
*   **Right:** Network information, bandwidth, and ping.

## Dependencies

*   `xclip`: Required for clipboard integration on WSL.

## Contributing

Feel free to open an issue or submit a pull request if you have any suggestions or improvements.

## License

This project is licensed under the MIT License.