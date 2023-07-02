# but-3-git-course

## L'aide de Git

Pour connaitre la version de Git installée sur votre machine, vous pouvez utiliser la commande suivante :

```bash
git --version
```

Pour connaitre la liste des commandes Git, vous pouvez utiliser la commande suivante :

```bash
git --help
```

Pour connaitre l'aide d'une commande Git, vous pouvez utiliser la commande suivante :
```bash
git help <command>
````

Par exemple, pour connaitre l'aide de la commande `git add`, vous pouvez utiliser la commande suivante :
```bash
git add --help
```

L'aide de git est aussi disponible en ligne à l'adresse suivante : https://git-scm.com/docs

Il est aussi possible d'avoir accès aux commandes avancées de Git en utilisant la commande suivante :
```bash 
git help -a
```

L'aide de Git sépare les commandes en plusieurs catégories :
- Main Porcelain : ce sont ces commandes qui sont utilisées le plus souvent, elles permettent de réaliser des actions de haut niveau, telles que l'ajout de fichiers, la création de commits, la création de branches, etc.
- Ancillary Commands : les commandes moins utilisées, mais qui sont utiles dans certaines situations

## Configuration de Git

Afin de vérifier la configuration de Git, vous pouvez utiliser la commande suivante :
```bash 
git config --list
```

Les configurations de Git sont stockées dans trois fichiers :
- `/etc/gitconfig` : contient la configuration de Git pour tous les utilisateurs et tous les dépôts
- `~/.gitconfig` : contient la configuration de Git pour un utilisateur et tous les dépôts
- `.git/config` : contient la configuration de Git pour un utilisateur et un dépôt


Il est possible de configurer Git en utilisant la commande suivante :
```bash
git config --global <key> <value>
```

Une des configurations les plus importantes est la configuration de     l'utilisateur. Il est nécessaire de configurer le nom et l'adresse email de l'utilisateur. Ces informations seront utilisées pour les commits. Cette configuration ce fait en utilisant les commandes suivantes :

```bash
git config --global user.name "John Doe"
git config --global user.email 
```
## Création d'un dépôt Git
Pour tout nouveau projet, il est nécessaire de créer un dépôt Git. Pour cela, il faut utiliser la commande suivante :
```bash
git init
```

Cette commande va créer un dossier caché `.git` qui va contenir tous les fichiers nécessaires au fonctionnement de Git.

Le dossier .git contient les éléments suivants :
- `config` : contient la configuration du dépôt Git
- `description` : contient la description du dépôt Git  
- `HEAD` : contient la référence vers la branche courante
- `hooks` : contient les scripts qui sont exécutés lors d'événements particuliers
- `info` : contient des informations supplémentaires
- `objects` : contient les objets Git
- `refs` : contient les références vers les commits

## Manipulation de fichiers et commit

Les fichiers peuvent être dans différents états :
- **Untracked** : le fichier n'est pas suivi par Git
- **Staged** : le fichier est suivi par Git et sera ajouté au prochain commit
- **Unmodified** : le fichier est suivi par Git et n'a pas été modifié
- **Modified** : le fichier est suivi par Git et a été modifié
- **Deleted** : le fichier est suivi par Git et a été supprimé
### Visualiser l'état des fichiers

Il est possible de visualiser l'état des fichiers avec la commande suivante :
```bash
git status
```

### Ajouter des fichiers dans l'index

Pour ajouter des fichiers, il faut utiliser la commande suivante :
```bash     
git add <file>
```

Il est possible d'ajouter tous les fichiers via la commande suivante :
```bash     
git add .
```

### Supprimer des fichiers de l'index

Pour supprimer des fichiers, il faut utiliser la commande suivante :
```bash 
git rm <file>
```
### Commiter des fichiers

Pour commiter des fichiers, il faut utiliser la commande suivante :
```bash 
git commit -m "Message du commit"
```

Le message du commit doit être explicite et doit décrire les modifications apportées par le commit. Il est possible de modifier le message du dernier commit en utilisant la commande suivante :
```bash
git commit --amend -m "Nouveau message du commit"
```

### Visualiser l'historique des commits

Pour visualiser l'historique des commits, il faut utiliser la commande suivante :
```bash
git log
```

Il est possible de visualiser l'historique des commits sous forme graphique avec la commande suivante :
```bash     
git log --graph
```

### Le fichier README.md

C'est le premier fichier que vous lisez lorsque vous arrivez sur un dépôt Git. Celui-ci permet de décrire le projet et de donner des informations sur le projet. Il est écrit en Markdown. Il est important de le compléter pour que les utilisateurs puissent comprendre le projet. 

Le site https://www.makeareadme.com/#suggestions-for-a-good-readme donne quelques conseils pour rédiger un bon README.md.

La page [markdown.md](./markdown.md) contient quelques informations sur la syntaxe Markdown.

### Le fichier .gitignore

Le fichier `.gitignore` permet de spécifier les fichiers qui ne doivent pas être suivis par Git. Il est possible de spécifier des fichiers, des dossiers, des extensions de fichiers, etc.

Le site https://www.gitignore.io/ permet de générer un fichier `.gitignore` en fonction du langage utilisé.
Github propose aussi une liste de fichiers `.gitignore` pour différents langages.


