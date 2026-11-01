<h1>Installation</h1>

L'installation ce fera sur un serveur d'entreprise Dell PowerEdge R420 sur l'hyperviseur Proxmox


### Prérequis
- Télécharger le fichier ISO depuis <a href="https://umbrel.com/downloads">le site d'Umbrel</a>
- Avoir accès au serveur Proxmox en LAN
- Sur Proxmox aller dans la partie "local (nom d'hôte)" --> "Images ISO", cliquer sur "Téléverser" et choissiser le fichier ISO
  

### Création de la VM

- Cliquer sur "Créer une VM"
<img width="229" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/371a1e7abf87831edfbeeb2e3ebb151073b8a1d7/img/01%20creer%20une%20vm.png"/>

- Préciser un nom pour la VM (ex. "UmbrelOS"), cocher la case "Avancé, puis cliquer sur le menu "vCPU architecture" et préciser x86 (64 bits). Umbrel os ne demarrera pas sinon
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/ccb90a81e0a4d4c6f7a6584a74d3225319ebaa4b/img/02%20general.png"/>

- Dans la section "Système d'exploitation, preciser le fichier ISO qu'on vien de téléverser dans la case "Image ISO". Laisser le reste par defaut.
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/bafe0c099abbe9b1ec2e6035198fbc4a104aa890/img/03%20systeme%20expl.png"/>

- **Important**: Dans "Système", selectionner OVMF (UEFI) et preciser l'emplacement du stockage EFI "local-lvm". **Sans cela, umbrelOS de pourra pas demarrer**
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/a912368c42900bc1502fe7d3326b0acc18d54906/img/04%20systeme.png"/>


- Partie "Disques" - prévoir au minimum 32 Go pour le système d'exploitation
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/fe020475d4a3f0a772d71626e1c2f587c0e60de1/img/05%20disques.png"/>

- Processeur ---> 4 Coeurs recommandé
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/dd94702f013cef89f06638ee781f1fc09ce97ad1/img/06%20processeur.png"/>

 
- Mémoire ---> minimum 4Go - 8 Go recommandé
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/8caee065b73f0f05eccc5c34e3e1984e81cc3469/img/07%20memoire.png"/>

- Réseau ---> préciser carte réseaux dans "Pont (bridge)" - cela nous donnera une adresse ip a nous connecter au server lorce qu'on le demarre
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/2c660aa45a3991c19f8edcf5be9105924ab5ec9c/img/08%20r%C3%A9seaux.png"/>

- Sur la dernière page, cliquer sur "Terminer"

### Mise en route de UmbrelOS

- Clique droit sur la VM ---> Cliquer sur "Démarrer"
- Se menu doit apparaitre
<img width="453" height="373" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/7555190b9a1afd9f07c80afde2dfdd693d6ccd24/img/2-01%20boot%20device.png"/>

- Avec les fleches du clavier, naviguer sur "EFI Firmware Setup" puis entrée


#### La VM se trouve actuellement dans le BIOS
- Naviguer sur "Device Manager" 
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/35e5df3f9b17e4894175107ace6a3dddb38eacf0/img/2-02%20bios.png"/>

- Sur "Secure Boot Configuration", descendre a l'option "Attempt Secure Boot" et appuyer sur Espace afin que la case n'est pas cochée
<img width="1506" height="1141" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/5e15a8b86f116c93cb13358c09fd17b209aa3911/img/2-03%20secure%20boot.png"/>
 
- Appuyer sur F10 puis Entrée pour sortir du BIOS et sauvegarder les modifications

#### UmbrelOS est désormais prêt a être installé
- Lorsque la VM se redémarrera, se menu apparetra
<img width="1942" height="1302" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/83a42167cb2984b6f49d54d8798bac1f08263f4f/image-installation.png" />

- Choisir sur quelle moyen de stockage installer umbrelOS a l'aide des touches du clavier de la liste, puis appuyer sur entrée

#### UmbrelOS est désormais installé
