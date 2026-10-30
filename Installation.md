<h1>Installation</h1>


- Télécharger le fichier ISO depuis <a href="https://umbrel.com/downloads">le site d'Umbrel</a>
- Utiliser une clé USB de minimum 32 Go avec <a href="https://etcher.balena.io/">BalenaEtcher</a> pour flasher le fichier ISO
- Choisir **EFI** avec **Secure Boot OFF**, ou l'installeur de demarrera pas.
- Choisir un 64-bit Linux si l'hyperviseur le demande.
- Configurer la carte réseau en "Bridge" donnera le nom de domaine "http://umbrel.local" au serveur.

## Criteres d'installation

- **Intel ou AMD :** 64-bit - Laptops, PC, NAS, ou Serveur. Minimum : Deux-Coeurs CPU, 4 GB RAM (8 GB+ conseillé), and a 32 GB drive for umbrelOS. umbrelOS boots from one drive and uses the rest for apps and data.
- **Raspberry Pi 5:** booter depuis une clé USB ou une carte microSD
- **Machine Virtuelle (VM):** Proxmox, VirtualBox, VMware - tout hyperviseur qui supporte "EFI boot"

 <img rc="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/64c3118ce06a819db38a66b61f8f7fbc3963ce46/image-garde-remplacer.jpeg" />
<img width="1942" height="1302" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/83a42167cb2984b6f49d54d8798bac1f08263f4f/image-installation.png" />

- Choisir sur quelle moyen de stockage installer umbrelOS a l'aide des touches du clavier de la liste"
