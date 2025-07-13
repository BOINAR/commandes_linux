# 🧠 Configuration du terminal Zsh (Linux / macOS)

Ce document regroupe les bases essentielles pour comprendre et personnaliser son terminal avec Zsh. Il est principalement basé sur la configuration du fichier `~/.zshrc`.

---

## 📁 1. Variables d’environnement

Les variables d’environnement permettent de définir des chemins ou des options accessibles globalement dans le terminal.

### Exemple :

```bash
export ANDROID_HOME="$HOME/Applications/android-studio/Sdk"
export PATH="$PATH:$ANDROID_HOME/platform-tools"
export PATH="$PATH:$ANDROID_HOME/emulator"
```

## Permet de modifier la configuration du terminal
```zsh
nano ~/.zshrc
```
## Permet de recharger le fichier sans fermer le terminal
```zsh
source ~/.zshrc
```

## 🪄 2. Alias utiles

Les alias permettent de raccourcir des commandes longues ou d’en créer de nouvelles. Ils se définissent comme ceci :

```bash
alias nom_alias='commande_originale'


# Ouvrir VS Code
alias codev='code .'

# Lister les fichiers avec détails et couleur
alias ll='ls -alh --color=auto'

# Mettre à jour les paquets sous Debian/Ubuntu
alias maj='sudo apt update && sudo apt upgrade -y'

# Naviguer rapidement
alias proj='cd ~/Documents/projets'

# Lancer Android Studio
alias studio='~/android-studio/bin/studio.sh'

# Redémarrer le shell Zsh
alias reload='source ~/.zshrc'

