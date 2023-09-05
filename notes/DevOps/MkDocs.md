
## Convertir du MarkDown en site web

Liens pour construire un site web via du MarkDown pour nos prises de notes par exemple.
- [MkDocs](https://www.mkdocs.org/)
- [Docusorus](https://docusaurus.io/fr/)

### MkDocs

1. Lancer un environnement virtuel python dans le projet.
	1. `python3 -m venv .venv`  -m pour dire que l'on crée le fichier ici, et .venv est le nom du fichier.
	2. `source .venv/bin/activate` pour se brancher sur l'environnement
2. `pip install mkdocs` pour installer mkdocs
3. `mkdocs new .` pour créer le nouveau projet
4. `mkdocs serve` pour lancer le serveur

> Bien mettre les .md dans le dossier Docs

1. Créer un projet Github
2. Lier son projet et push sur le répository Git
3. Lancer  `mkdocs gh-deploy`
4. Settings -> Pages -> Et HOP.
