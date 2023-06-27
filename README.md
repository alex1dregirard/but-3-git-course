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

Il est aussi possible d'avoir accès aux commandes avancées de Git en utilisant la commande suivante :
```bash 
git help -a
```

Afin de vérifier la configuration de Git, vous pouvez utiliser la commande suivante :
```bash 
git config --list
```

Il est possible de configurer Git en utilisant la commande suivante :
```bash
git config --global <key> <value>
```

Par exemple pour configurer le nom et l'adresse email de l'utilisateur, vous pouvez utiliser les commandes suivantes :
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

### Visualiser l'historique des commits

Pour visualiser l'historique des commits, il faut utiliser la commande suivante :
```bash
git log
```

Il est possible de visualiser l'historique des commits sous forme graphique avec la commande suivante :
```bash     
git log --graph
```


