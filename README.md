# Netflix RSS Reader

Projet d'AL consistant à implémenter le RSS Reader de Netflix avec Docker

## Installation

L'installation du RSS Reader est assez simple et rapide, selon le vitesse de connexion

### Cloner le repo

Commencez par gloner ce repo dans le dossier de votre choix

```
git clone https://github.com/TReboux/AL
```

### Build les images

Descendez dans le dossier du repo et construisez les images

```
cd AL
sudo docker build -t eureka:latest eureka
sudo docker build -t middletier:latest middletier
sudo docker build -t edge:latest edge
```

## Lancer le serveur

Vous pouvez maintenant lancer le serveur avec la commande suivante

```
sudo docker-compose up
```

## Accéder au serveur

Le RSS Reader est maintenant accessible [ici](http://localhost:9090/jsp/rss.jsp)

Vous pouvez maintenant ajouter des flux RSS, par exemple celui de [la section politique du Washington Post](http://feeds.washingtonpost.com/rss/politics)
