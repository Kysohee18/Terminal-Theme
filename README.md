# TokyoNight HTB Terminal Theme

A high-performance, aesthetic terminal customization specifically designed for pentesting and long coding sessions. This theme merges the deep, soothing tones of **Tokyo Night** with the vibrant, cyber-security focused neon accents of **Hack The Box (HTB)**.

## 🎨 Overview

*   **Theme Name:** TokyoNight HTB
*   **Base Style:** TokyoNight Storm/Deep Blue
*   **Accent:** HTB Neon Green (`#9ece6a`) & Cyan (`#7dcfff`)
*   **Vibe:** Cyberpunk, Stealth, Professional.

## 🛠 Specifications

### 1. Color Palette

| Role | Hex Code | Description |
| :--- | :--- | :--- |
| **Background** | `#1a1b26` | Deep Blue (TokyoNight Storm) - Easy on the eyes for night sessions. |
| **Foreground** | `#a9b1d6` | Soft Blue-Grey - High contrast without harshness. |
| **Primary Accent** | `#9ece6a` | **HTB Green** - Used for success states, prompts, and key indicators. |
| **Secondary Accent** | `#bb9af7` | Purple - Adds depth to visual hierarchy. |
| **Cursor** | `#c0caf5` | Block cursor with blinking effect. |
| **Selection** | `#33467c` | Subtle prominence. |

### 2. Typography

*   **Font Family:** [JetBrains Mono Nerd Font](https://www.nerdfonts.com/font-downloads) or [Iosevka](https://typeof.net/Iosevka/).
*   **Size:** 11pt - 13pt.
*   **Line Height:** 1.2.
*   **Features:** Ligatures enabled (e.g., `->` becomes an arrow), Nerd Font Icons required for glyphs.

### 3. Shell Prompt (Oh My Posh)

This repository includes a `theme.json` configuration for **Oh My Posh**.

*   **Structure:** `[Icon OS] [Current Directory] [Git Branch] [Execution Time]`
*   **Separators:** Minimalist Powerline symbols or clean spacing.
*   **Right Prompt:** Shows language versions (Python/Go) and Time. *Recommendation: Add VPN IP/tun0 status for pentesting context.*

### 4. Visual Effects

To achieve the intended "glassmorphism" or futuristic look:

*   **Opacity:** 0.85 - 0.90 (Slight transparency).
*   **Blur:** Gaussian Blur enabled (requires Windows Terminal, Alacritty, or iTerm2).
*   **Padding:** 15px - 20px internal padding.

## 📦 Recommended Tooling

To complete the experience, ensure your CLI tools match the aesthetic:

1.  **Neovim:** Install `folke/tokyonight.nvim`.
2.  **LS_COLORS:** Use `vivid` to generate a compatible LS_COLORS theme.
3.  **Shell:** Zsh syntax highlighting enabled (Green for valid commands, Red for invalid).

## 🚀 Installation

1.  **Install Oh My Posh:** Follow the [official documentation](https://ohmyposh.dev/docs/installation).
2.  **Download Theme:** Clone this repo or download `theme.json`.
3.  **Apply Configuration:**
    Add the following to your shell profile (e.g., `.zshrc` or PowerShell `$PROFILE`):

    ```powershell
    oh-my-posh init pwsh --config 'path/to/theme.json' | Invoke-Expression
    ```

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
