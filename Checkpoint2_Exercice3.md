### Q.3.1
- Matériel réseau A : Switch
- Assurer la connectivité entre les ordinateurs du réseau.

### Q.3.2
- Matériel B est un Routeur
- Assurer le routage entre le réseau local et d'autres réseaux.

### Q.3.3
- f0/0 : Interface de B connectée à un réseau local.
- g1/0 : Interface de B connectée à un autre réseau.

### Q.3.4
- /16 dans l'adresse IP de PC2 signifie que les 16 premiers bits sont utilisés pour identifier le réseau, les 16 autres sont pour les hôtes de ce réseau.

### Q.3.5
- L'adresse 10.10.255.254 est l'adresse de passerelle

### Q.3.6
- Pour PC1 :
  - Adresse de réseau : 10.10.0.0
  - Première adresse disponible : 10.10.0.1
  - Dernière adresse disponible : 10.10.255.253
  - Adresse de diffusion : 10.10.255.254
- Pour PC2 :
  - Adresse de réseau : 10.11.0.0
  - Première adresse disponible : 10.11.0.1
  - Dernière adresse disponible : 10.11.255.253
  - Adresse de diffusion : 10.11.255.254
- Pour PC5 :
  - Adresse de réseau : 10.10.0.0
  - Première adresse disponible : 10.10.0.1
  - Dernière adresse disponible : 10.10.255.253
  - Adresse de diffusion : 10.10.255.254

### Q.3.7

### Q.3.8
- Aucun des ordinateurs du schéma ne peut atteindre le réseau 172.16.5.0/24 car aucune route n'est configurée pour ce réseau.

### Q.3.9

### Q.3.10
  - Utiliser un serveur DHCP pour attribuer dynamiquement les adresses IP aux ordinateurs.

## Analyse de trames

### Fichier 1 :

#### Q.3.11
l'adresse MAC : 00:50:79:66:68:00

#### Q.3.12


#### Q.3.13

oui il a eu une réponse
![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex3/Capture%20d'%C3%A9cran%202024-05-17%20131505.png)

source ip : 10.10.4.1 mac: 00:50:79:66:68:00
destination : 10.10.4.2 mac : 00:50:79:66:68:03

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex3/Capture%20d'%C3%A9cran%202024-05-17%20131505.png)

#### Q.3.14

le protocole encapsulé est ARP : Address Resolution Protocol

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex3/Capture%20d'%C3%A9cran%202024-05-17%20131517.png)

#### Q.3.15

Son role a été de trouver l'adresse Mac correspondant à une adresse IP
### Fichier 2 :

#### Q.3.16
l'adresse : 10.10.80.3 demarre cette communication 

#### Q.3.17

le protocole est ICMP et son role est la gestion du trafic et la communication entre les hôtes et les routeurs sur Internet

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex3/Capture%20d'%C3%A9cran%202024-05-17%20131416.png)

#### Q.3.18
Non il n'a pas eu de réponse du destinataire

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex3/Capture%20d'%C3%A9cran%202024-05-17%20132504.png)

#### Q.3.19
il envoie un requete  au destinataire par le protocole ICMP et la destination est introuvable.

#### Q.3.20


### Fichier 3 :

#### Q.3.21
source 10.10.4.2 est un reseau privé local
destination 172.16.5.253 est un réseau privé

#### Q.3.22
source : ca:01:da:d2:00:1c
destination : ca:03:9e:ef:00:38

#### Q.3.23
