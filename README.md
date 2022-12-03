Créer un annuaire pour le site Assurez-vous que vos fichiers HTML se trouvent déjà dans le répertoire actif. 
Créer un fichier appelé Dockerfile Placez le contenu suivant dans le Dockerfile FROM nginx:alpin COPY. /usr/share/nginx/html Ces lignes de code représentent l’image que nous allons utiliser avec la copie du contenu du répertoire actuel dans le conteneur. 
Créer l’image Docker pour le serveur HTML Exécutez la commande suivante : Docker build . Vous pouvez confirmer que cela a fonctionné en exécutant la commande : Docker Images
Creer un fichier nginx.conf pour la configuration
 Exécutez la commande suivante pour exécuter le serveur de conteneur HTML : Docker run -d -p puis le port(80:80) puis le nom de l'image Exécutez la commande suivante pour vous assurer que le serveur est en cours d’exécution : curl localhost:80
  Vous pouvez également le voir dans le navigateur maintenant en allant à localhost: 80 et vous devriez voir votre fichier HTML.