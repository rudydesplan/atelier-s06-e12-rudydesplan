# atelier-s06-e12

Sur votre vm cloud serveur, installez l'applicatif writefreely. https://github.com/writefreely/writefreely

## Instructions d'installation

Réinstallez votre vm cloud server pour avoir une base propre (et au passage on sera tous en Ubuntu 22.04).

Utilisez l'archive tar.gz correspondant à l'architecture de votre cloud serveur (amd64) sur https://github.com/writefreely/writefreely/releases/tag/v0.14.0

Il doit être installé avec un compte utilisateur (student), le serveur doit être installé en mode "Production, standalone" et "Insecure (port 80)", il faut le configurer pour utiliser un serveur MySQL. Vous pourrez modifier le port d'écoute ultérieurement vers le port 8080.

Lancez et testez le service depuis votre poste de travail.

Vous devez avoir votre service qui s'affiche via http://<pseudoGithub>-server.eddi.cloud:8080

## Configurer un service systemd

Utilisez systemd et définissez un service pour pouvoir gérer l'exécution de votre blog avec systemctl <stop/restart/start> blog.

## Notifiez votre formateur pour vérification

Maintenant que vous avez un service fonctionnel il est temps d'effectuer une correction afin de voir si vous avez utilisé la bonne méthode.

## Pour aller plus loin quand vous avez fini.

En configurant Nginx Apache ou Caddy en reverse proxy, rediriger le flux vers le port 80 entrant.

Configurez un certificat Letsencrypt dans Apache/NGinx/Caddy pour rendre disponible votre blog en https.

