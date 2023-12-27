# lab-osint

## Préparation du lab

* Installation de Kali Linux: iso téléchargeable (https://www.kali.org/get-kali/#kali-platforms)

-> disponible pour i64 et ARM (mac M1 & M2)

* Puis une fois installé, mise à jour des dernièrs paquets:

```
sudo apt update
```

```
sudo apt upgrade --yes
```

## Emails

### Holehe

Un excellent outil qui sert à rechercher des informations depuis un email. 

* Pour l'installation:

```
sudo apt install pip3
```

```
sudo pip3 install python-slugify
```

```
sudo pip3 install holehe
```

* Puis pour l'utilisation:

```
holehe test@gmail.com
```

### Turbolehe:

Turbolehe est une extension qui se greffe sur Holehe et qui va vous permettre d’améliorer vos enquêtes OSINT grâce à une recherche pas nom + prénom, ainsi que de la génération de rapports. 

* Toutes les dépendances nécessaires à Turbolehe sont déployées, on va installer l'outil depuis son dépot git:

```
git clone https://github.com/UserCr4ig/Turbolehe
```

puis se rendre dans le répertoire nouvellement créé, Turbolehe

* Enfin pour une recherche, c'est très simple:

```
python3 turbolehe.py NOM PRENOM
```

On peut cibler un domaine:

```
python turbolehe.py NOM PRENOM -B
```

### haveibeenpwned

Une base de données des emails apparaissant dans des listes sur les blackmarkets. Si on est dedans, c'est mauvais signe...

https://haveibeenpwned.com/

## Nom de domaine

### Dig / whois

Un domaine regorge d'informations importantes. Bien souvent c'est caché par l'opérateur. Sous Kali on peut utiliser l'outil dig

Exemple: `dig scourzic.net`

Whois est également accessible depuis plusieurs sites, pour obtenir des informations publiques.

### Onyphe

Ce site va plus loin, notament sur le scan de sous domaines: https://www.onyphe.io/

$${\color{green}TP}$$

D'après mon site, trouvez des informations sur un autre sous domaine que j'héberge, qui lui même vous mènera à mon adresse email.

A partir de celle ci vous effectuerez une recherche pour trouver un ou plusieurs service(s) auxquels je suis abonné.









