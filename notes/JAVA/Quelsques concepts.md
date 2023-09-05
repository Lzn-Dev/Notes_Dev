
### Les mots clés :

```Java
==> volatile : Une variable "volatile" est une variable pour laquelle la JVM garantie que l on récupèrera toujours une valeur à jour.
Utile dans 2 cas :
	- Lorsque la mise à jour d une variable ne dépend pas de sa valeur précédente. Par exemple pour le cas d un flag d initialisation du genre isReady.
	- Lorsqu il n y a qu un seul Thread qui modifie la variable (les autres ne faisant que la lire).
```


### La généricité :

``` Java

---------------- ArrayList<E> ------------------

La classe générique c est le fait de pouvoir créer une "ArrayList<>();" de quelque chose. De typé les éléments que va contenir notre "ArrayList"
Exemple :
- ArrayList<String> : Liste de String
- ArrayList<Logement> : Liste de logements
-  ...

Convention des noms de types :
<T> => Type
<E> => Element
<K> et< V> => Key et Value
<N> => Number
<?> => JOKER

----------------- Methode générique --------------

public static <T> void methode (T obj) {
// Methode générique qui prend en paramètre un objet de type T
}


public static <T> T methode(T obj) {
// Methode générique qui retourne l'objet de type T
}

public static <T extends Personne> void methode(T obj) {
// Méthode générique qui attend un objet de type Personne ou une
// sous classe à Personne.
}

// On peut faire "extends" d'une classe mais aussi d'une interface pour
//avoir accès aux méthode de cette interface en plus des methodes de classes
//"Object".

------------------ Classe générique ---------------------

public class Generic <T> {
	private T obj;

	public Generic(T obj) {
		this.obj = obj;
	}

	public T getObj() {
		return obj
	}
}
// Ou en extends :
public class Generic <T extends Personne> {
// ...
}

Personne p1 = new Personne();
Generic<Personne> genericPersonne = new Genericc<Personne>(p1);

------------------- JOKER ---------------------

Comment créer une méthode avec uyn parametre de type de classe générique ?
private static void print (ArrayList<?> liste) {
/// ...
}

private static void methode (Generic<? extends Hote> arg) {
/// ...Au moins de ce type la ou une fille
}

private static vvoid methode (Generic<? super Hote> arg) {
/// ... Au mieux de ce type la ou une mère
}

```

### Les classes immuables

``` Java

"Mutable" = Quelque chose qui peut évolué
( On peut en changer ses valeurs )
---- VS ----
"Immutable" = Qui ne peut pas évolué
( Se dit des types de variable qui ne peuvent pas changer pendant lexécution du programme )

------------- DEFINITION ----------------

Une classe définie sans possibilité de mutation.
Cela permet de créer une 'classe' avec l 'assurance que ces instances ne puissent pas changer' de valeurs pour leurs champs.
Java permet de garantir l immuabilité en déclarant les champs final

-------------- Exemple -----------------

private final int x;
private final int y;

-------------- Avantages ----------------

- Un seul état
- Facile à créer , tester
- "thread-safe"
- Leurs valeurs de hachage reste fixe et peut même être mise en cache une fois calculée dans le constructeur : ilssont donc à privilégier dans les collections de type Map et Set.

------------ Copie défensive -------------

private final StringBuilder name;

// Pour se proteger d'un :
// StringBuilder nomDeChat = new StringBuilder("Sylvestre");
// MaClasse exemple = New MaClasse(nomDeChat);
// nomDeChat.reverse();
// exemple.getName() => Retourne "ertsevlyS";
public MaClasse(StringBuilder name) {
	this.name = new StringBuilder(name);
}

// On double la copie défensive au getter pour se proteger de :
// nomDeChat.getName().reverse() => "ertsevlyS"
public StringBuilder getName() {
	return new StringBuilder(name);
}

```

### Classe anonyme

```Java
Le fait de faire un new sur une interface ou sur une class abstract permet de mettre en place une classe anonyme.
Il faut alors mettre le corp de la classe ou de l interface à la suite du code :

Interface interface = new Interface() {
	@overide
	public void maMethodeInterface() {
		// ...
	}
}

```

### Expression lambda
```Java
On utilise des Interfaces Fonctionelles pour cela, des interfaces à une seule méthode.

On notera en annotation :

@FunctionnalInterface
interface MonInterface() {
	// ...
}
```

![Texte alternatif](file:///Users/matthieu/Desktop/Screenshots/Capture%20d%E2%80%99e%CC%81cran%202023-03-24%20a%CC%80%2009.55.05.png)

### Interface fonctionelle

```Java
Par definition une interface fonctionnelle est une interface qui ne contient qu une et unique methode.

```


### Interface graphique

```Java
JFrame en Java pour l interface graphique
```

### Paamayim Nekudotayim

```Java
Se renseigner, c est l operateur "::"
```

### Streams

```Java
=> Permet de gérer des collection via la classe "Stream";

Ex :
Stream<Integer> stream = Stream.of(new Integer[]{1, 2, 3, 4});
stream.forEach(p -> System.out.println(p));

=> On peut aussi appliquer le stream à une liste déja existante :
List<String> maListe = new ArrayList<>();

maListe.stream().filter(nom -> nom.startWith("A"));

```
