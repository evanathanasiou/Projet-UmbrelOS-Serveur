<h1>Installation</h1>

L'installation ce fera sur un serveur d'entreprise Dell PowerEdge R420 sur l'hyperviseur Proxmox


# Prérequis
- Télécharger le fichier ISO depuis <a href="https://umbrel.com/downloads">le site d'Umbrel</a>
- Avoir accès au serveur Proxmox en LAN
- Sur Proxmox aller dans la partie "local (nom d'hôte)" --> "Images ISO", cliquer sur "Téléverser" et choissiser le fichier ISO
  

Création de la VM

- Cliquer sur "Créer une VM"
<img width="229" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/371a1e7abf87831edfbeeb2e3ebb151073b8a1d7/img/01%20creer%20une%20vm.png"/>

- Préciser un nom pour la VM (ex. "UmbrelOS"), cocher la case "Avancé, puis cliquer sur le menu "vCPU architecture" et préciser x86 (64 bits). Umbrel os ne demarrera pas sinon
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/ccb90a81e0a4d4c6f7a6584a74d3225319ebaa4b/img/02%20general.png"/>

- Dans la section "Système d'exploitation, preciser le fichier iso qu'on vien de téléverser dans la case "Image ISO". Laisser le reste par defaut.
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/bafe0c099abbe9b1ec2e6035198fbc4a104aa890/img/03%20systeme%20expl.png"/>

- **Important** Dans "système", selectionner OVMF (UEFI) et preciser l'emplacement du stockage EFI "local-lvm". **Sans cela, umbrelOS de pourra pas demarrer**
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/a912368c42900bc1502fe7d3326b0acc18d54906/img/04%20systeme.png"/>


- Partie "Disques" - prévoir au minimum 32 Go pour le système d'exploitation
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/fe020475d4a3f0a772d71626e1c2f587c0e60de1/img/05%20disques.png"/>

- Processeur ---> 4 Coeurs recommandé
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/dd94702f013cef89f06638ee781f1fc09ce97ad1/img/06%20processeur.png"/>

 
- Mémoire ---> minimum 4Go - 8 Go recommandé
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/8caee065b73f0f05eccc5c34e3e1984e81cc3469/img/07%20memoire.png"/>

- Réseau ---> préciser carte réseaux dans "Pont (bridge)" - cela nous donnera une adresse ip a nous connecter au server lorce qu'on le demarre
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/2c660aa45a3991c19f8edcf5be9105924ab5ec9c/img/08%20r%C3%A9seaux.png"/>


 <img rc="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/64c3118ce06a819db38a66b61f8f7fbc3963ce46/image-garde-remplacer.jpeg" />
<img width="1942" height="1302" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/83a42167cb2984b6f49d54d8798bac1f08263f4f/image-installation.png" />
- Choisir sur quelle moyen de stockage installer umbrelOS a l'aide des touches du clavier de la liste
