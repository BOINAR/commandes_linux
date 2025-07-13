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


