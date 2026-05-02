# Kitty.conf-Gentoo
🐱 Kitty + Starship + Fastfetch — Config Gentoo

> Configuration personnalisée pour un terminal moderne et élégant sous Gentoo Linux.

![Gentoo](https://img.shields.io/badge/Gentoo-Linux-54487A?style=flat-square&logo=gentoo&logoColor=white)
![Kitty](https://img.shields.io/badge/Terminal-Kitty-F5A97F?style=flat-square)
![Starship](https://img.shields.io/badge/Prompt-Starship-DD0B78?style=flat-square&logo=starship&logoColor=white)
![ZSH](https://img.shields.io/badge/Shell-ZSH-89DCEB?style=flat-square)

---

## 📦 Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- [Kitty](https://sw.kovidgoyal.net/kitty/) — Terminal GPU-accelerated
- [ZSH](https://www.zsh.org/) — Shell recommandé
- [Starship](https://starship.rs/) — Prompt cross-shell
- [Fastfetch](https://github.com/fastfetch-cli/fastfetch) — Affichage des infos système

### Installation des prérequis sur Gentoo

```bash
emerge --ask app-shells/zsh app-misc/fastfetch
emerge --ask x11-terms/kitty
emerge --ask app-shells/starship

⚙️ Installation
1. 🐱 Configuration Kitty

mkdir -p ~/.config/kitty
nano ~/.config/kitty/kitty.conf

    Colle le contenu du fichier kitty.conf puis sauvegarde.

2. 🚀 Configuration Starship

mkdir -p ~/.config
nano ~/.config/starship.toml

    Colle le contenu du fichier starship.toml puis sauvegarde.

Assure-toi d'avoir ajouté Starship à ton ~/.zshrc :

eval "$(starship init zsh)"

3. ⚡ Configuration Fastfetch

mkdir -p ~/.config/fastfetch
nano ~/.config/fastfetch/config.jsonc

    Colle le contenu du fichier config.jsonc puis sauvegarde.

🔄 Appliquer les changements

source ~/.zshrc

📁 Structure du dépôt

Kitty.conf-Gentoo/
├── kitty.conf          # Config du terminal Kitty
├── starship.toml       # Config du prompt Starship
├── config.jsonc        # Config de Fastfetch
└── README.md

🖼️ Aperçu

    Screenshot à venir

📄 Licence

Projet open-source — libre d'utilisation et de modification.
