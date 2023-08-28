## Les quatres fondamentaux de la POO :
### L'abstraction 
- Exemple : Pour conduire une voiture, on utilise les pédales, le levier de vitesse et le volant ***sans avoir besoin*** de connaître le fonctionnement interne exacte de la voiture.
- Les avantages : 
	- Reduire la complexité.
	- Eviter la duplication.
 - Une classe qui ne peut pas être instancié. 
 - Une méthode abstraite est définit vide dans le parent, et oblige ses filles à redéclarer cette méthode.
### L'héritage 
- Mécanisme pour définir  une nouvelle classe comme extension d'une classe préexistante. 
- La classe *fille* hérite également du comportement (méthodes) de la classe *mère*.
- Le mot clé *extends* à la définition de classe, ne permet que l'héritage simple. 
- L'héritage par implémentation. 
	- Une classe peut hériter de 0, 1 ou plusieurs interfaces par implémentation. 
	- Mot clé *implements* à la définition de la classe, ne permet que l'héritage d'interface. 
 - Rajouter l'annotation @Override quand on redéfinit une méthode de la classe parente dans la classe enfant. 
 - Il existe une classe, nommé Object, qui est la mère de toutes les classes. De base si l'on crée une classe, le compilateur rajoutera extends Object. Si la classe n'hérite pas déjà d'une autre classe.
### L'encapsulation
- Le fait d'enfermer et de masquer à l'intérieur d'une classe : 
	- Les données
	- L'implémentation des méthodes
### Polymorphisme 
- Une capacité de la programmation orienté objet permettant de maniper un objet sous un type plus général que le sien. 
- C'est grâce à l'héritage que le polymorphisme existe. 
- Un objet peut apparaître sous un type plus général que le sien, c'est à dire sous la forme de sa classe mère. 

### Les mots clés :
#### This. : 
- Permet de parler d'une instance précise d'une classe. Celle que l'on modifie à l'instant T.
#### Static :
- Qui est partagé. => On va pouvoir utilisé ce mot clé devant un attribut.
- *Ce n'est pas lié aux instances mais à la classe elle même.*
- Si un objet modifie la valeur de l'attribut, il sera modifié pour tout les objets. 
	- Ex :
```java
public static int longueur;
// La largeur sera partagé entre toutes les instances de la classe terrain.
public static void initLongueur(int value) {
	longueur = value;
	// Ici ce n'est pas this.longueur, si on l'écris ça ne compilerait pas. C'est la classe et non l'instance qui est impacté. 
}
```
- On manipulera donc cet attribut non depuis l'instance mais depuis la classe.
- Idem les *methodes statiques* sont directement associées à la classe et non aux instances de la classe.
#### Final :
- Indique qu'un élément ne peut être changé dans las uite du programme.
- On dit qu'il est non modifiable que ce soit par lui ou par des éventuelles sous classes.
- Il doit *obligatoirement* être initalisé.
- A le rôle d'une CONST 
- Personne dans le programme ne pourra alterer la donnée. 





### Interface
- Une interface est une Type *complétement abstraite*
- C'est une liste de promesses 
- Lorsqu'une classe tient les promesses d'une interface on dit que la classe implémente l'interface
- Particularités :
	- Une classe peut implémenter plusieurs interfaces
	- Les interfaces peuvent hériter les unes des autres
	- On peux faire des setter protected pour laisser le droit au filles mais mettre des conditions. 

### Exceptions
- Définition : circonstance endant la poursuite de l'éxecution inutile ou impossible ( erreur dans les données, défaillance materielle ... ).
- Principe du mécanisme :
	1. Détection de l'anomalie 
	2. La méthode lance (throw) l'exception vers celle qui l'a appelé
	3. L'exceptionremonte
	4. Jusqu'a une méthode ou on a prévu d'attrapé ( catch ) l'exception
