<h1>Accès et configuration</h1>

UmbrelOS est accessible en webadmin, pour y accéder, il faut trouver l'adresse IP attribué

- Lorsque la VM se demarre, se menu apparaitra
<img width="229" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/34ecc43c558063fc3ee02ed806d1939dbbb0a614/img/3-01%20login.png"/>

- Saisir l'utilisateur et mot de passe par defaut - umbrel / umbrel

#### UmbrelOS est désormais en mode "Terminal access"
<img width="665" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/2d9d6fee48411836d6cb0e94aa272dbdf4192bd9/3-02%20terminal.png"/>

- Saisir la commande suivante:

```
ip -br -4 addr
```

- Noter l'adresse IP qui se situe sur l'interface e#### (ex. ens18)
<img width="665" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/37459f2a4b3e637a4691395e4bf2b95c92c7cbe8/3-03%20ip.png"/>

- Sur un autre poste, saisir l'adresse IP noté dans un navigateur (ex. https://192.168.1.13)

#### La page suivante s'affichera
<img width="665" height="665" alt="bento 2 0" src="https://github.com/evanathanasiou/Projet-UmbrelOS-Serveur/blob/02e91c9e2701ef0f99b23da50d762e3d642f08f4/img/3-04%20setup.png"/>

- En cliquant sur "Get Started", on peut choisir un nom d'utilisateur et confirmer deux fois le mot de passe
