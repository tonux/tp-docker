TP Docker: Déploiement du site mon CV

0-) Se connecter sur le terminal

1-)  ## Vérifier si docker est installé
--> docker --version

2-) ## Créer l'image Docker
docker build -t nom:tag .

Ex: docker build -t tp:1.0.0 .

3-)  ## Afficher la liste des images
--> docker images

4-) ## Démarrer le Container Docker sur le port 8080
docker run -d -p 8080:8080 tp:1.0.0

Ex: docker run -d -p 8080:8080 tp:1.0.0

5-)  ## Vérifier le status des Container
--> docker ps

6-) Ouvrir votre navigateur, aller sur l'url http://localhost:8080/

7-) ## Arrêter le Container Docker
--> docker stop CONTAINER_NAME

8-) ## Supprimer l'image 
-> docker rm IMAGE_NAME
