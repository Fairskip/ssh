## Challenge

Fournir un fichier de configuration valide pour un serveur OpenSSH permettant la configuration suivante :

<br>

- Le serveur écoute sur le port TCP 222 en IPv6 uniquement

```
 # Choix du port TCP sur lequel le serveur écoute - 22 par défaut
 Port 22

 # Écoute sur toutes les interfaces IPv6
ListenAddress ::
```

<br>

- Seul l'utilisateur ayant le nom de login `wilder` peut se connecter

```
 # Liste d'utilisateurs pouvant se connecter 
 AllowUsers fairskip
```

<br>

- La connexion par mot de passe est impossible. Une clé est nécessaire.

```
# Authentification par mots de passe - valeur par défaut yes 
PasswordAuthentication no

# Authentification par clés - valeur par défaut yes 
PubkeyAuthentication yes
```

<br>

## Resultat 

<img src = https://github.com/Fairskip/ssh/blob/main/Log%20in%20via%20Mobaxter.jpg width = "2500" height = "200">
