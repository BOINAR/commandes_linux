# Commandes linux

#### Nivagation & fichier

```zsh
pwd : # affiche le repertoire de travail
```

```zsh
cd : # naviguer dans le systeme
```

```zsh
mkdir : # créer un répertoire
```

```zsh
ls : # voir contenu des répertoires
```

```zsh
mkdir : # créer un répertoire
```

```zsh
touch : # créer un fichier // expemple touch bonjout.txt
```

```zsh
mv : # renommer un fichier // expemple mv bonjout.txt salut.txt // déplace le fichier au meme endroit en le renommant
```

```zsh
cp : # copier un fichier // expemple touch bonjout.txt repertoire // déplace le fichier à l'intérieur du dossier répertoire
```

```zsh
rm : # supprime un fichier // expemple rm bonjout.txt
```

```zsh
rm -r : # supprime un dossier // expemple rm -r repertoire
```

```zsh
cat : # afficher le contenu d'un fichier // expemple cat bonjout.txt
```

```zsh
grep : # recherche une chaine dans un fichier
```

```zsh
grep -r : # Cherche le mot dans tous les fichiers du dossier courant et dans tous ses sous-dossiers, et dans les fichiers qu’ils contiennent, etc.
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

#### Gestion des paquet (APT)

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










