# Installation docker

## Pré-requis

1. Docker
2. Nginx

## Procédure

### Service user

1. Créer un dossier, `users` par exemple
2. Mettre le fichier [docker-compose.yml](https://github.com/La-Nouvelle-Epoch-18/lne-user/blob/master/docker-compose.yml) dans le dossier
3. Éxecuter la command `docker-compose pull` dans le dossier (accès root peut être nécéssaire avec sudo)
4. Éxecuter la command `docker-compose up -d` dans le dossier (accès root peut être nécéssaire avec sudo)
   
Le service est opérationnel

---
### Service posts

1. Créer un dossier, `posts` par exemple
2. Mettre le fichier [docker-compose.yml](https://github.com/La-Nouvelle-Epoch-18/lne-posts/blob/master/docker-compose.yml) dans le dossier
3. Éxecuter la command `docker-compose pull` dans le dossier (accès root peut être nécéssaire avec sudo)
4. Éxecuter la command `docker-compose up -d` dans le dossier (accès root peut être nécéssaire avec sudo)
   
Le service est opérationnel

---
### Service channels

1. Créer un dossier, `channels` par exemple
2. Mettre le fichier [docker-compose.yml](https://github.com/La-Nouvelle-Epoch-18/lne-channel/blob/master/docker-compose.yml) dans le dossier
3. Éxecuter la command `docker-compose pull` dans le dossier (accès root peut être nécéssaire avec sudo)
4. Éxecuter la command `docker-compose up -d` dans le dossier (accès root peut être nécéssaire avec sudo)
   
Le service est opérationnel

---
### Site web

1. Créer un dossier, `front` par exemple
2. Mettre le fichier [docker-compose.yml](https://github.com/La-Nouvelle-Epoch-18/lne-front/blob/master/docker-compose.yml) dans le dossier
3. Éxecuter la command `docker-compose pull` dans le dossier (accès root peut être nécéssaire avec sudo)
4. Éxecuter la command `docker-compose up -d` dans le dossier (accès root peut être nécéssaire avec sudo)
   
Le site est opérationnel
