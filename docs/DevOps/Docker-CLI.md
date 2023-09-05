# Command Line Docker

- Build de l'image (A partir d'un Dockerfile)
`docker build . -t nom-image`

- Liste les images
`docker image ls`

- Attribut un tag à l'image =>
`docker tag image_id nom_du_tag`

- Inspecte l'image =>
`docker inspect id_image`

- Sauve une image dans une archive | -o pour output
`docker save id_image -o nom_fichier.tar nom_image:tag nom_image2:tag`

- Supprimer une image `-f` pour forcer la suppression
`docker image rm id_image`

- Charger une image depuis une archive `--input` pour lire un fichier .tar
`docker load --input nom_fichier.tar`

- Liste les containers en cours d'execution
`docker ps`

- Liste tous les container
`docker container ps -a`

- Avoir les informations d'un utilisateur | -rm pour dire au container de se supprimer après éxécution
`docker run --rm id_image id nom_user`

- Lancer un conteneur spécific
`docker start conteneur_id`

- Stopper un conteneur spécifi
`docker stop conteneur_id`


