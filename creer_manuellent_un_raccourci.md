Créer un fichier .desktop
 
 1. À quoi sert ce fichier .desktop ?
Un fichier .desktop est un raccourci d'application dans les systèmes Linux avec interface graphique (comme GNOME, KDE, etc.).
Il sert à :

Lancer une application

L’afficher dans le menu des applications

L’épingler dans le dock

Lui associer une icône

Et plus encore (raccourcis, actions personnalisées, etc.)

### Exemple :

```zsh
nano ~/.local/share/applications/android-studio.desktop
```
```zsh
[Desktop Entry]                 # Indique que c’est un fichier de type "desktop"
Version=1.0                    # Version du fichier (pas de l'app)
Type=Application               # Type = application (peut aussi être Link, Directory, etc.)
Name=Android Studio            # Nom visible dans le dock / menu
Exec=/chemin/vers/studio.sh    # Chemin de lancement de l'app (script ou binaire)
Icon=/chemin/vers/studio.png   # Icône affichée (chemin absolu recommandé)
Terminal=false                 # Doit-on ouvrir un terminal pour lancer ? (false ici)
Categories=Development;IDE;    # Catégories pour classement dans le menu
StartupNotify=true             # Affiche une animation pendant le lancement
```

🔐 Pourquoi chmod +x ?
Par défaut, un fichier .desktop n’est pas exécutable, donc :

Il n’apparaît pas dans le menu des applications

Tu ne peux pas le lancer en double-cliquant

👉 chmod +x permet de donner les droits d’exécution au fichier.
C’est une sécurité de Linux pour éviter qu’un fichier de type .desktop non vérifié puisse s’exécuter sans ton consentement.
```zsh
chmod +x ~/.local/share/applications/android-studio.desktop
```

🔐 chmod = CHange MODe
chmod est une commande qui sert à modifier les permissions d’un fichier ou d’un dossier.

🧠 Sur Linux, chaque fichier a des permissions :
Ces permissions définissent qui peut faire quoi :

Permission	Signification
r (read)	Lire le fichier
w (write)	Modifier / écrire
x (execute)	Exécuter (comme un programme ou un script)

Et elles s’appliquent à trois types d’utilisateurs :

Catégorie	Signification
u (user)	Le propriétaire
g (group)	Le groupe du fichier
o (others)	Tous les autres utilisateurs

📌 Les opérateurs dans chmod
Symbole	Signification	Exemple
+	Ajoute une permission	chmod +x → ajoute x (exécution)
-	Supprime une permission	chmod -w → enlève w (écriture)
=	Remplace complètement les droits	chmod =r → met seulement r


🧱 Structure : 1 + 3 + 3 + 3
Bloc	Signification
-	Type du fichier (- = fichier, d = dossier)
rwx	Propriétaire (user / owner)
r--	Groupe (group)
r--	Autres utilisateurs (others)

Donc dans -rwxr--r-- :

- → c’est un fichier

rwx → le propriétaire peut lire (r), écrire (w), exécuter (x)

r-- → les membres du groupe peuvent seulement lire

r-- → tout le reste du monde peut seulement lire

