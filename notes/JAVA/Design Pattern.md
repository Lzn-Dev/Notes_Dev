
```Java

------ TODO ------

Créer des mix de pattern pour s entrainer
Factory Builder
Singleton Builder


Les design patterns répondes à certaines problèmatique de conception en différentes catégories :
=> Création
	- Factory = Créer des instances filles d une classe
	- Builder = Créer une instance immuable
	- Singleton = Créer une classe avec une instance unique
=> Structure
=> Comportement


============ CRÉATION ============

---------- Singleton -----------

Ce design pattern permet de créer "une et unique" instance de classe.
Cette unique instance est un attribut de la classe elle-même.
Bien souvent, l objectif en plus de cette unicité, est de pouvoir y acceder depuis partout dans le programme.

---------- Builder -----------

- Création d une classe interne static nommée Builder.
- Cette classe a un constructeur avec les attributs obligatoire et des méthodes pour les attributs optionnels
- Le constructeur de la classe devient private. Et prend en paramètre une instance de ce Builder.
- Une méthode "build" dans le Builder est définie afin de créer une instance


=============== STRUCTURE ==============

---------- Proxy ----------

Un objet "proxy" qui cache l objet d origine
Permet de "cacher une instance" en manipulant seulement l instance de la classe proxy
Utilisé afin d ajouter une sécurité
	- Une interface "Subject" pour définir les fonctionnalités
	- Une classe "RealObject"
	- Une classe "ProxyObject" qui extends "RealObject"

--------- Adapter ----------

Classe qui établit le lien entre deux instances qui ne savent pas communiquer au premier abords.
"C est le chargeur entre la prise et l ordinateur "


=============== COMPORTEMENT ==============

----------- Strategy -----------


----------- State -----------

- Designe qui integre une interface qui definit les états possibles d un composant
