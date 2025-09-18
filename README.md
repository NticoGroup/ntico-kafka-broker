## Lancer Kafka en Local avec Docker Compose

Ce document fournit les instructions nécessaires pour lancer **Kafka**, **ZooKeeper** et **Kafka UI** en local à l'aide de Docker Compose.

-----

### Description

Ce dépôt (`ntico-kafka-broker`) fournit une configuration **`docker-compose`** simple pour lancer un environnement local composé de **Kafka**, **ZooKeeper** et **Kafka-UI**. Cet outil est parfait pour le développement et les tests, car il permet de mettre en place rapidement tous les services nécessaires pour interagir avec Kafka.

-----

### Prérequis

Assurez-vous que les éléments suivants sont installés sur votre machine :

  * **Docker Desktop** : Inclut Docker Engine et Docker Compose. Vous pouvez le télécharger depuis le [site officiel de Docker](https://www.docker.com/products/docker-desktop/).
  * **Ce dépot** : Vous aurez besoin de cloner ce dépot.

-----

### Utilisation

Pour démarrer les services, commencez par **cloner le dépôt Git** sur votre machine.

#### 1\. Démarrer les services

Naviguez dans le répertoire cloné :

```bash
cd ntico-kafka-broker
```

Ensuite, exécutez la commande suivante pour démarrer les services :

```bash
docker compose up -d
```

Cette commande télécharge les images nécessaires et démarre les conteneurs en arrière-plan.

-----

### Commandes

#### Accéder à Kafka UI

Une fois les services démarrés, vous pouvez accéder à l'interface de Kafka UI via votre navigateur à l'adresse suivante :

[http://localhost:8082](http://localhost:8082)

#### Arrêter les services

Pour arrêter et supprimer les conteneurs, utilisez la commande :

```bash
docker compose down
```
