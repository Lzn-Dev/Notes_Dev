
### Spring, qu'estce que c'est ? 

- Créer des applications Web - Java
	- + Configuration trés simple
	- + Clés en main
	- + Application robuste et facilement maintenable 
	- + Gestion de la configuration
	- + Injection de dépendances ( Le coeur de Spring )
	- + Grosse communautée 

Le site pour commencer un projet en Spring : start.spring.io 
- Spring web en "Add dependencies" en starter 

### Les grands concept 

#### Injection de dépendances :
- Permet de fournir à une classe toutes les dépendances dont elle va avoir besoin pour effectuer ses tâches. 
- Pas besoin à une classe d'instancier elle même les éléments dont elle a besoin.

#### IoC ( Inversion of Control )
- Concept de Spring qui facilite la gestion des dépendances entres les différentes classes de l'application. 
- Cela permet de déléguer à Spring, la création et l'initialisation de classes dans un conteneur IoC.
	- + Injection des dépendances automatique à l'éxécution.
	- + Réduction de la complexité.
	- + Maintenabilité accrue.
- C'est l'*IoC* qui va contenir toutes nos dépendances. 


#### Serialisation / Désérialisation ( Jackson )
Désérialisation => 
- Format stockable (Json, ...) => Objet JAVA
- Il faut un constructeur vide par defaut dans la classes.
- Et des setters.
Sérialisation => 
- Objet JAVA => Format stockable (Json, ...)
- Il faut des getter.




