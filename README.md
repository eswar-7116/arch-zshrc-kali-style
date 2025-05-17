# 🐧 Custom `.zshrc` for Arch Linux (Kali-Inspired)

A powerful, clean, and functional `.zshrc` configuration tailored for Arch Linux users — inspired by the aesthetics and utility of Kali Linux terminals. Comes with plugin integrations, useful aliases, and enhanced visuals.

## 🚀 Features

- ⚙️ **oh-my-zsh** framework support
- 🔌 Plugin support:
  - `zsh-autosuggestions`
  - `zsh-syntax-highlighting`
  - `you-should-use`
  - `extract`
  - `web-search`
  - `colored-man-pages`
- 🧠 Minimal and efficient alias setup
- 🎨 Colorized prompt and improved CLI UX
- ✅ Tested to work smoothly even with Python virtual environments (`.venv`)

## 📸 Preview

![Screenshot](https://github.com/user-attachments/assets/b8f75374-9aac-4c04-8fd7-3306664195f4)

## 🧰 Requirements

Ensure the following are installed on your system:

- **Zsh** (`zsh`)
- **Oh My Zsh** (`oh-my-zsh`)
- **Required Plugins** (install via Git or package manager):
  - `zsh-autosuggestions`
  - `zsh-syntax-highlighting`
  - `you-should-use`
  - `web-search`
  - `extract`
  - `colored-man-pages`
- **Fonts**:
  - [Nerd Font](https://www.nerdfonts.com/font-downloads) (any variant)
  - [Noto Color Emoji](https://fonts.google.com/noto/specimen/Noto+Color+Emoji)

## 🔧 Setup

- Install Zsh

```bash
sudo pacman -S zsh
```

- Use `curl` and `git` to install `oh-my-zsh` and other plugins:
```bash
# Install curl if not installed
pacman -S git curl

# Install Oh My Zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Clone required plugins
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/you-should-use

git clone https://github.com/zsh-users/zsh-autosuggestions \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

- Apply this .zshrc:
```bash
curl -s https://raw.githubusercontent.com/eswar-7116/arch-zshrc-kali-style/refs/heads/main/.zshrc > ~/.zshrc
```
- Finally, restart your terminal or run:
```bash
source ~/.zshrc
```

### ⭐ Star this repo if you find it helpful!
