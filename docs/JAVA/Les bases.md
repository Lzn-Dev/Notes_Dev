
## Origine 
- Créé par James Gosling vers 1995 chez Sun Microsystems
- Destiné à l'informatique répartie : sécurité, réutilisabilité, portabilité 
	- Langage neuf ( pas de comptabilité à assurer )
	- Langage orienté objets
	- bibliothèquye très importante
	- Langage compilé et interprété 

## Introduction 
Java est compilé et interprété 
- Compilation : Traduction texte java -> Bytecode
- Interprétation : Exécution du bytecode par une machine virtuelle Java

### Mon premier programme :
- Le programme *HelloWorld.java* : 
	```java
	public class HelloWorld {
		public static void main(String[] args) {
			System.out.println("HelloWorld");
			/* Commentaire sur plusieurs 
			lignes.
			*/

			// Sur une seule ligne
		}
	}
	```
**Le Nom du programme `HelloWorld.java` est important, il porte le même nom que la classe du fichier**

### Les variables | Types primitifs 
- Une variable possède un nom, un type et une valeur.
```Java
int a;
a = 5;
```
- Il est ensuite possible de changer la valeur 
```Java
int a = 5;
a = 21;
```
*En Java, le symbole `=` désigne l'affectation et n'a pas la même signification qu'en mathématiques.*

- Les nombres entiers : 
	- Byte : 8bits
	- Short : 16bits
	- Int : 32bits
	- Long : 64bits - Rajouter un l ( L minuscule ) en fin de valeur 
- Les nombres décimaux
	- Float : 32bits - Rajouter un f en fin de valeur
	- Double : 64bits
 - Booleans
	 - Booleans : 1bits ( Initialisé à false )
- Les caractères
	- char : 16bits

## Tips 
### Le else if : 
- Le else if n'est rien d'autre qu'un `else` suivi d'un `if` indenté de manière à simplexifier le code :
``` java
// Premier IF
else {
	if (true) {
	System.out.print('LALA')
	}
}

// Est égal à ===>

else if (true) {
	System.out.print('LALA')
}
```

- La boucle foreach en Java ! 
```Java
for (String s : numberAsArray) {  
    System.out.println("-----> " + Integer.parseInt(s));  
}
```



## Raccourcis InteliJ
- SO => Pour System.out.....