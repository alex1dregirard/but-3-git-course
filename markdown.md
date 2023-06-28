# markdown

Markdown est un langage de balisage léger créé en 2004 par John Gruber avec l'aide d'Aaron Swartz. Son but est d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été marqué par des balises ou des instructions de formatage, comme c'est le cas, par exemple, avec du texte enrichi (par exemple du HTML).

## Syntaxe

Plus de détail sur le site [markdownguide](https://www.markdownguide.org/basic-syntax/)

### Titres

Pour créer un titre, il faut utiliser le caractère `#` suivi du titre. Il est possible d'utiliser jusqu'à 6 caractères `#` pour créer un titre de niveau 6.

```markdown 
# Titre de niveau 1
## Titre de niveau 2
```

### Paragraphes

Pour créer un paragraphe, il faut écrire le texte du paragraphe sur une seule ligne.

```markdown 
Ceci est un paragraphe.
```

### Italique

Pour mettre du texte en italique, il faut entourer le texte avec le caractère `*` ou `_`.

```markdown
*Texte en italique*
_Texte en italique_
```

### Gras

Pour mettre du texte en gras, il faut entourer le texte avec le caractère `**` ou `__`.

```markdown
**Texte en gras**
__Texte en gras__
```

### Italique et gras

Pour mettre du texte en italique et en gras, il faut entourer le texte avec le caractère `***` ou `___`.

```markdown     
***Texte en italique et en gras***
___Texte en italique et en gras___
```

### Barré

Pour barrer du texte, il faut entourer le texte avec le caractère `~~`.

```markdown
~~Texte barré~~
```

### Listes

Pour créer une liste, il faut utiliser le caractère `-` ou `*` suivi du texte de l'élément de la liste.

```markdown
- Élément 1 
- Élément 2
```

### Listes ordonnées

Pour créer une liste ordonnée, il faut utiliser le caractère `1.` suivi du texte de l'élément de la liste.

```markdown     
1. Élément 1
2. Élément 2
```

### Listes imbriquées

Pour créer une liste imbriquée, il faut utiliser le caractère `-` ou `*` suivi du texte de l'élément de la liste.

```markdown
- Élément 1
  - Élément 1.1
  - Élément 1.2
- Élément 2
```

### Listes imbriquées ordonnées

Pour créer une liste imbriquée ordonnée, il faut utiliser le caractère `1.` suivi du texte de l'élément de la liste.

```markdown
1. Élément 1
   1. Élément 1.1
   2. Élément 1.2   
2. Élément 2
```

### Liens

Pour créer un lien, il faut utiliser le caractère `[` suivi du texte du lien, puis du caractère `]` suivi de l'URL du lien entre parenthèses `()`.

```markdown
[Texte du lien](https://www.google.com)
```
### Images

Pour insérer une image, il faut utiliser le caractère `!` suivi du caractère `[` suivi du texte alternatif de l'image, puis du caractère `]` suivi de l'URL de l'image entre parenthèses `()`.

```markdown 
![Texte alternatif](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)
```

### Code

Pour insérer du code, il faut utiliser le caractère ` (Alt Gr + 7) pour insérer du code sur une ligne ou le caractère ``` pour insérer du code sur plusieurs lignes.

Il existe plusieurs convertisseurs Markdown:
    
### Tableaux

Pour créer un tableau, il faut utiliser le caractère `|` pour séparer les colonnes et le caractère `-` pour séparer la première ligne du reste du tableau.

```markdown
| Colonne 1 | Colonne 2 |
| --------- | --------- |
| Ligne 1   | Ligne 1   |
| Ligne 2   | Ligne 2   |
```

### Citations

Pour créer une citation, il faut utiliser le caractère `>` suivi du texte de la citation.

```markdown 
> Ceci est une citation.
```

#### Notes de bas de page

Pour créer une note de bas de page, il faut utiliser le caractère `[^]` suivi du texte de la note de bas de page.

```markdown
Ceci est un texte avec une note de bas de page.[^1]

[^1]: Ceci est une note de bas de page.
```



