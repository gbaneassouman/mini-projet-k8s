  # Mini Projet Kubernetes
  <div align="center"><img src="images/wp_k8s.png"></div><br/>
  Ce Projet denommé mini projet Kubernetes a été réalisé dans le cadre de mon      parcours **Devops** au **Bootcamp N°15 de EAZYTraining**.  
  
  ## Objectifs

 Il s'agit ici de deployer **WordPress** à l'aide manifest selon les informations ci-dessous: 
- Créer un objet de type Deployment pour MySQL avec un seul replicas 
- Créer un objet de type Service de type **clusterIP** pour exposer le **Pod MySQL**
- Créer un objet de type Deployment avec un seul replicas pour **WordPress** avec les paramètres de connexion à **MySQL**
- Les données de WordPress seront stockées dans le répertoire /data du Noeud
- Créer un service de type **NodePort** pour exposer **WordPress**

## Get Started 🚀  

J'ai apporté un changement en ajoutant un **Namespace** pour cloisonner l'application WordPress (voir ci-dessous).

## Architecture 

<div align="center"><img src="images/wp-k8s-31.png"></div>


## Tâches réalisées
1 - Deploiement de l'environnement k8s
2 - Ecriture des manifests necessaires au deploiemnt de **Wordpress**
3 - Deploiement de **Wordpress**

## Plan de Travail

### 1 - Installation de l'environnement k8s

Comme environnement j'ai opté pour **Minikube et VirtualBox** pour la réalisation de ce projet.

- Téléchargement et installation de **Minikube**
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube

```
- Démarrage

```
minikube start --driver=virtualbox

```
