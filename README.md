# Commandes linux

#### Navigation & fichier

```zsh
pwd : # affiche le repertoire de travail
```

```zsh
cd <dossier> : # naviguer dans le systeme
```

```zsh
mkdir <dossier> : # créer un répertoire
```

```zsh
ls : # voir contenu des répertoires
```

```zsh
touch <fichier> : # créer un fichier // expemple touch bonjout.txt
```

```zsh
mv <src> <dest> : # renommer un fichier // expemple mv bonjout.txt salut.txt // déplace le fichier au meme endroit en le renommant
```

```zsh
cp <src> <dest> : # copier un fichier // expemple touch bonjout.txt repertoire // déplace le fichier à l'intérieur du dossier répertoire
```

```zsh
rm <fichier> : # supprime un fichier // expemple rm bonjout.txt
```

```zsh
rm -r <dossier> : # supprime un dossier // expemple rm -r repertoire
```

```zsh
cat <fichier> : # afficher le contenu d'un fichier // expemple cat bonjout.txt
```

```zsh
grep "<mot>" <fichier> : # recherche une chaine dans un fichier
```

```zsh
grep -r "<mot>" . : # Cherche le mot dans tous les fichiers du dossier courant et dans tous ses sous-dossiers, et dans les fichiers qu’ils contiennent, etc.
```

```zsh
ps : # verifier les processus en cours
```

```zsh
ls -la : # liste les fichier / affiche les détails / Affiche aussi les fichiers cachés --color=auto
Coloration (souvent activée automatiquement)
```

```zsh
ls -a : # affiche tous les fichiers et dossiers, y compris les fichiers cachés (ceux qui commencent par un .), ainsi que . (dossier courant) et .. (dossier parent).
```

```zsh
history # Affiche ton historique de commandes
```


#### Editeur de test 

```zsh
nano <fichier> : # Éditeur de texte simple dans le terminal
vim <fichier> : # Éditeur plus avancé (à apprendre plus tard si besoin)
code . : # Ouvre le dossier courant dans VS Code (si installé avec WSL)
```

#### Shell & scripts

```zsh
echo "texte" : # Affiche du texte
cat <fichier> : # Affiche le contenu d’un fichier
head <fichier> : # Affiche les premières lignes
tail <fichier> : # Affiche les dernières lignes
history : # Montre l’historique des commandes
!! : # Réexécute la dernière commande
Ctrl + R : # Recherche dans l’historique
bash <script.sh> : # Exécute un script bash
```

#### Gestion des paquets (APT)

```zsh
sudo apt update : # Met à jour la liste des paquets
sudo apt upgrade : # Met à jour les paquets installés
sudo apt install <paquet> : # Installe un paquet
sudo apt remove <paquet> : # Supprime un paquet
apt search <terme> : # Cherche un paquet
dpkg -l : # Liste les paquets installés
```

#### Droits & permissions

```zsh
chmod +x <fichier> : # Rend un script exécutable
chown <utilisateur>:<groupe> <fichier> : # Change le propriétaire d’un fichier
sudo : # Exécute une commande avec les droits admin
```

#### 🌐 Réseau

```zsh
ping google.com :Vérifie la connexion réseau
curl <url> : Récupère une page ou API (utile en dev)
wget <url> : Télécharge un fichier via HTTP
ip a : Affiche les interfaces réseau (comme ifconfig)
```











