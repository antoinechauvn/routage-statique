# routage-statique
Approfondissement du routage statique

Le routage statique permet donc à l'administrateur de saisir manuellement les routes sur les routeurs et ainsi de choisir lui même le chemin qui lui semble le meilleur pour aller d'un réseau A à un réseau B

Lorsque vous ajoutez une adresse IP à une interface et que cette interface est active, la route est ajoutée à la table de routage.

1. Configuration d’une route statique
```
(config)#ip route <network> <mask> {address|interface} [AD]
```
* network : est l’adresse du réseau à joindre
* mask : est le masque du réseau à joindre
* address : est l’adresse du prochain routeur directement connecté pour atteindre le réseau
* interface : est l’interface de sortie du routeur pour atteindre le réseau
* AD : distance administrative optionnelle (1, par défaut)

![image](https://user-images.githubusercontent.com/83721477/167009712-bd2be6c5-a021-4cc8-a9b7-491d1513a299.png)
* `C` : Connected<br>
* `S` : Static
