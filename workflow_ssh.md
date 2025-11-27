
# Workflow pour connexion vers un serveur en ssh

## créer la clé ssh

```zsh
ssh-keygen -t ed25519 -C "ton-email"
```

### configurer alias dans ~/.ssh/config

```zsh
Host nomduhost
HostName adresseip
User root (root ou nom du user)
IdentityFile ~/.ssh/id_ed25519
IdentitiesOnly yes
AddKeysToAgent yes
UseKeychain yes

```

### charger la clé

```zsh
ssh add ~/.ssh/id_ed25519
```

ssh nomduhostdanslaconfig

### Création du user non-root :

```zsh
adduser nayeff
usermod -aG sudo nayeff
```

Depuis le Mac ou le pc, installer la clé SSH directement sur l’utilisateur final (et pas root) :

```zsh
ssh-copy-id -i ~/.ssh/id_ed25519.pub nomdelutilisateurcréé@adresseipduserveur
```

###	Vérifier les permissions côté VPS (en tant que nayeff) :

```zsh
chmod 700 ~/.ssh
chmod 600 ~/.ssh/authorized_keys
chown -R nayeff:nayeff ~/.ssh
```

### 8.	Modifier l’alias sur le Mac pour utiliser nayeff :
```zsh
Host contabo
  HostName 194.163.177.96
  User nayeff
  IdentityFile ~/.ssh/id_ed25519
  IdentitiesOnly yes
  AddKeysToAgent yes
  UseKeychain yes
```

  - tester

    ```zsh
    ssh contabo
    connexion sans mot de passe, directement sur nayeff
    ```

### 	10.	Désactiver root SSH :

```zsh
sudo nano /etc/ssh/sshd_config
# PermitRootLogin no

sudo systemctl restart ssh
```






