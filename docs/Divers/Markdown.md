# Markdown

>Markdown est un langage de balisage léger créé en *2004* par **John Gruber** avec l'aide d'Aaron Swartz, dans le but d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été balisé ou formaté par des instructions particulières.


## Les titres 
```mixed
#  Titre 1
## Titre 2
###  Titre 3
#### Titre 4
#####  Titre 5
###### Titre 6
--------------
Titre 1
=
```

## Le texte
```mixed
*Texte en italique*
_Texte en italique_
**Texte en gras**
__Texte en gras__
***Texte en italique et en gras***
___Texte en italique et en gras___
~~Texte barré~~
```

*Texte en italique*
**Texte en gras**
***Texte en italique et gras***
~~Texte Barré~~

## Les citations
```mixed
>Ceci est une **zone en retrait**.
>La zone continue ici

>Ceci est une autre **zone de retrait**.
Cette zone continue également dans la ligne suivante.
Cependan, cette ligne n’est plus en retrait
```

>Ceci est une **zone en retrait**.
>La zone continue ici

>Ceci est une autre **zone de retrait**.
Cette zone continue également dans la ligne suivante.
Cependan, cette ligne n’est plus en retrait

## Les listes
```mixed
UL : Choix entre '+', '-', '*'
- Liste1
- Liste2
- Liste3

OL 
1. Liste 1
2. Liste 2
3. Liste 3

Liste à cocher
[ ] A
[x] B
[ ] C
```
**Astuce** : *Le chiffre employé n’a aucune importance pour Markdown. Que vous écriviez trois fois le chiffre 1, ou que vous commenciez par le chiffre 3, le langage Markdown rédigera dans tous les cas une liste correctement numérotée.*

## Code
```mixed
`<h1>Hello World</h1>`
```

`<h1>Hello World</h1>`

## Images et hyperliens
```mixed
Lien :
Ici ce qui suit [MonSuperLien](https://example.com/ "titre de lien optionnel").
Image :
![Ceci est un exemple d’image](https://cdn.pixabay.com/photo/2018/07/29/23/05/woman-3571298_1280.jpg)
Lien + Image :
[![Ceci est un exemple d’image](https://example.com/bild.jpg)](https://example.com)
```
Ici ce qui suit [MonSuperLien](https://example.com/ "titre de lien optionnel").

![Ceci est un exemple d’image](https://cdn.pixabay.com/photo/2016/11/30/20/58/programming-1873854__480.png)

## Les tableaux

*Les **barres verticales** (|) permettent d’éditer des tableaux avec Markdown. Chaque cellule du tableau est séparée d’une barre verticale. Pour créer des lignes de titre qui se distinguent du reste du tableau, vous devrez souligner les cellules concernées avec les tirets du 6.*

```mixed
|cellule 1|cellule 2|
|--------|--------|
|    A    |    B    |
|    C    |    D    |
```






