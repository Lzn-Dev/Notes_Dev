### Table d'Audit Trail : Sauvegarde de donnée en base.

## Les différents types de donnée :

1. Alphabétique         =>       "toto"
2. Numérique             =>       "1234"
3. Alphanumérique    =>       "toto1234"
4. Binaire                    =>        "01100101101010"
5. Temporelle             =>        "26-12-2021"
6. Spatiale                  =>        Se renseigner


## BDD No SQL == Not Only SQL
1. => Format JSON
2. Couple => Clé/Valeur

Base de donnée avec des données structurées et d'autre non. L'un n'empêche pas l'autre.

## Normes :

- Qui est le propriétaire ? ( des données )
	- Exemple : Facebook (Meta) en 2009 : Quand les utilisateurs postaient une photo, elle devenait la propriété de Facebook (Meta).

*Classifion les données :*
- Anonyme
- Rendu anonyme
- Pseudonomisé
- Identifiante
- Données d'exploitation

*Sensible à une norme ? :*
- Donnée personelle
- Banque
- Santé
- RH
- Défense
- ....

*Propriété intellectuelle ? :*
- Protégé : patrimoine de l'entreprise
- Droits auteurs
- ....

*La notion de territoire et de portage des donnée*
- Respecter le cadre juridique du pays dans lequelle les données vont être exploitées
- Respecter le cadre de transfere de donnée d'un pays à l'autre


## Infrastructure

**Questions à ce poser :**
- Flux entrants : Les acteurs chargent / envoient bcp de données
- Flux sortants : les acteurs extraient bcp de données
- Traitement processeur : Requêtes compliquées / Fréquente
- Espace de stockage : Volume de données stockées.


## Sécurité

**A l'intérieur :**
- Flux entrants / sortants : Canal de communication chiffré ? Entre qui et qui ? App <-> DB | User <-> DB ?
- Protection des accès : Qui se connecte ? Humain | Machine ? De ou ? Filtrage IP ou autre. Qui accède phusiquement ?
- Espace de stockage : Volume / Fichiers chiffrés ( niveau disque ) ? media (raid)
- Surface d'attaque : Bloquer la disponibilité du site suivant le pays ( par adresse IP )

**A l'extérieur :**
- Protection des accès : GRANT
- Les données : Chiffrées (niveau moteur de DB) ?
- Traçabilité : Journalisation, Audit Trail
- Intégrité : Transaction
- Risques : Injections ou manipulations

RGPD => Droit à l'oublie .

## Sauvegarde

**Quel plan ? :**
- RPO : Recovery Point Objective : Si nous devons restaurer, quelle fraicheur dce donnée souhaitons nous ?
- RTO : Recovery Time Objective : SI nous devons restaurer, combien de temps avons nous ?

***Une sauvegarde n'est considérée valable si et uniquement si un plan de test de restauration a été fait et est documenté***

## Archivage

- Combien de temps ? Cycle de vie de la donnée ( Qui dit : elle meurt, quand ... )
- A quelle endroit ? Sur quel media ? Qui accede ?
- Attention au transfert vers le lieuy d'archivage
- Quelle garantie souhaitée ? Société d'archivage professionnelle ?


## Maintenance

- Disponibilité : Mieux vaut une sonde de monitoring qui vous prévient d'une défaillance qu'un utilisateur insatisfait qui vous appelle.
- La croissance / volume : Quelle est l'évolution dela croissance ? Quelle est la limite fixée au départ ?
