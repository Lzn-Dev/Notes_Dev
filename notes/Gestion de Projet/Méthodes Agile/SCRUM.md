# SRUM
***Terme du Rugby pour dire "Une mêlée"

## La théorie

### Définition :
- Cadre méthodologique pour développer les produits complexes :
	- Rôles, évènements, artefact et règles.
- Le savoir est basé sur l'expérience.
- Prise de décision sur ce qui est connu.
- Ce fait en cycle de "Sprint" de 1 à 4 semaines.

#### Les 3 pilliers :
- Transparence.
	Confiance mutuelle et la compréhension entre équipe et management
- Vérification continue, Inspection
	Les variation indésirable entre les objectifs et le produit sont régulièrement évaluées par l'équipe.
- Adaptation
	Si l'inspection détecte les dérives, lréquipe se réunit lors de "rituel" afin de modifier sa façon de travailler (processus)


### Les différents rôles :
**Product Owner => PO**
- Maximiser la valeur du produit
- Gère le Product Backlog (Priorité)
	- En détail :
		- *Responsable ultime* du produit et de ses caractéristiques (qualités)
		- *Représente l'organisation client* et les utilisateurs du produit
		- Prend les *décisions stratégiques et tactiques* liées au produit
		- *Définit et priorise les objectifs* en lien avec le produit
		- *Partage* sa vision du produit
		- Possède une *excellente connaissance du métier*
		- Gère les *feedbacks des utilisateurs* liées à l'utilisation et aux changements du produit
		- *Optimise* la valeur du produit dans l'entreprise

**Equipe de développement**
- Auto-gérée.
- Réalise le développement.
	- En détail :
		- Composée de *3 à 9* personnes maximum aux compétences variées et complémentaires afin d'optimiser l'efficacité.
		- Ils *développent* et *délivrent* à chaque *Sprint* un porduit appelé **incrément**, potentiellement utilisable.
		- *Pluridisciplinaire* et *compétente*.
		- *Responsable de la qualité du développement* du produit.

**Le scrum master => SM**
- Faire adhérer l'équipe à la théorie, aux pratique et aux règles.
- Facilitateur
- C'est l'arbitre
	- En détail :
		- Responsable de la *bonne application* de la méthode Scrum
		- Aide au quotidien l'équipe à *mettre en oeuvre Scrum* sur le projet
		- Comme *coach*, il aide l'équipe à développer ces compétences Scrum
		- Comme *mentor*, il suggère des idées et préconise des améliorations
		- Aide à la *planification* du produit et du projet
		- *N'est pas un chef de projet* et n'a pas de pouvoir hiérarchique sur l'équipe de développement

### Les cérémonies
***Cérémonie Scrum : Sprint ( timebox d'un mois max)***
- Sprint Planning
	- => Définir l'objectif du Sprint, Analyser et évaluer le Product Backlog
	- En collaboration avec toute l'équipe
- Daily scrum ( 15 minutes )
	- Ce qui a été fait hier, ce qui va être fait aujourd'hui pour contribuer à l'atteinte de l'objectif, points de blocage.
- Sprint Review ( Revue à la fin du sprint )
	- Ce qui a été fait et non fait, mise à jour du Product Backlog.
- Sprint Rétrospective
	- Amélioration des méthodes utilisées ( personne, relation, processus, outils )


### Les artefacts
***Eléments tangibles***
- Représentant du travail ou de la valeur
- Fournissant de la visibilité à l'intérieur et à l'exterieur de l'équipe ( Transparance )
- Facilitant l'inspection et l'adaptation

### Release
***X.Y.Z => X : Major , Y : Minor , Z : Patch***
***Exemple : 1.4.3***

**Une release a deux sens distincts :**
	1. Version délivrée d'un porduit
	2. Période de temps nécessaire à la production de ce produit
- L'ensemble des sprints d'un produit forme une *release*
- Un *incrément* est une partie d'un produit utilisable
	- Les *incréments* se cumulent dans un Sprint


### Poker Planning
- Séance d'estimation de l'effort nécessaire au développement de chaque Item du produit backlog.
- Menée par la team en utilisant un jeu de carte prenant des valeurs d'estimation ainsi qu'une carte supplémentaire "?" en cas d'impossibilité à estimer.
- Le resultat de l'affiche s'exprime en Story Point.
- Les valeurs des cartes du planning poker :
	- 0 , 1/2 , 1 , 2 , 3 , 5 , 8 , 13 , 20 , 40 , 100 , ?
- Chacun des acteurs choisis une carte, la retourne face caché et la découvre,  en même temps que les autres, ainsi les choix ne sont pas biaisés et la discussion part de ce point.


## Glossaire
- *Product Backlog* : Carnet de produit géré par le PO => Liste ordonée, priorisé et exhaustive d'items (éléments), ou de stories à développer par l'équipe.
- *Items* : Chaque item inclut une description, une priorité, une estimation de l'effort et la valeur apporté. Les items peuvent être des :
	- Features ( Caractéristiques )
	- Besoins
	- Améliorations
	- Correctifs ( bugs )
- Epics, Themes, Features, Stories
- Definition of Done
- Release Plan
- Sprint Backlog
- Taskboard
- Tasks
- Potentially Shippable Product Increment
- Velocity
- Release Burndown
- *User Story* : Formalisé comme suit :
	- En tant que ( As a .. ) -> Rôle
	- Je veux ( I want .. )  -> Fonctionnalité
	- Afin de ( So that .. ) -> Valeur
	- Exemple : *En tant que* client *je veux* télécharger ma facture *afin de* la payer par CB sur internet
- *INVEST* pour Indépendante Négociable Valorisable Estimable Small Testable
