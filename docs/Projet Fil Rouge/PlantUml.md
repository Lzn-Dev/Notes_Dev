
### Code source diagramme de sequence
#### Partie 1 :
```
@startuml

actor Utilisateur

==Accueil==

Utilisateur -> Site: Visualisation de l'agenda
opt Filtrer agenda
    Utilisateur -> Site: Filtre selon des critères
end
Site -> Back: Requête
Back -> BDD: Requête
BDD --> Back:
Back --> Site:
Site --> Utilisateur: Affichage

Utilisateur -> Site: Sélectionne une date
Site -> Back: Requête page formulaire
Back -> BDD: Requête disponibilité des salles
BDD --> Back:
Back --> Site: Code couleurs suivant les salles
Site -> Utilisateur: Renvoi vers la page de formulaire

== Page formulaire ==

Utilisateur -> Site: Renseigne les champs
Site -> Utilisateur: Règles métiers
alt Validation formulaire
    Utilisateur -> Site: Valide le formulaire
    Site -> Back: Requête
    Back -> BDD: Requête pour reserver la salle
    alt Salle disponible
        BDD -> BDD: Réservation salle
    else Salle non disponible
        BDD -> BDD: En attente de validation
    end
    BDD --> Back:
    Back --> Site:
    Site --> Utilisateur: Message information
else Annulation
    Utilisateur -> Site: Annule la réservation
    Site -> Back: Redirection page d'accueil
    Back -> BDD: Requête
    BDD --> Back:
    Back --> Site:
    Site --> Utilisateur: Retour page d'accueil
end

@enduml
```

#### Partie 2

```
@startuml

actor Utilisateur

alt Est admin
==Dashboard==

Utilisateur -> Site: Accès au dashboard
Site -> Back: Requête
Back -> BDD: Requête
BDD --> Back:
Back --> Site:
Site --> Utilisateur: Affichage des infos

Utilisateur -> Site: Sélectionne une entité
Site -> Back: Requête page crud
Back -> BDD: Requête
BDD --> Back:
Back --> Site:
Site -> Utilisateur: Renvoi vers la page crud

== Page Crud==

Utilisateur -> Site: Choisit une action du Crud
alt Modifier / Ajouter
    Site -> Utilisateur: Affiche le formulaire
    Utilisateur -> Site: Renseigne les champs
    Site -> Site: Verification champs
    Site -> Back: Requête
    Back -> BDD: Requête
    alt Succès
        BDD -> BDD: Ajout/Modification
    end
    BDD --> Back:
    Back --> Site:
    Site --> Utilisateur: Message d'informations

else Supprimer
    Utilisateur -> Site: Supprimer
    Site -> Utilisateur: Demande de confirmation
    Utilisateur -> Site: Réponse
    alt Confirmé
        Site -> Back: Requête
        Back -> BDD: Requête
        BDD -> BDD: Suppression
        BDD --> Back:
        Back --> Site:
        Site --> Utilisateur: Message de confirmation
    end

end
end

@enduml
```
