### Q.1.1



![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Ping_vers_Client.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Ping_vers_Serv.png)

le ping du client au serveur ne fonctionne par car ils sont sur des sous-réseaux différents.
- le Client est en 172.16.100.50/24

 |adresse      |adresse de réseau |adresse de diffusion | masque sous réseau|plage d'adresses des hotes |
 |:-----------:|:----------------:|:-------------------:|:-----------------:|:-------------------------:|
 |172.16.100.50|172.16.100.0      |172.16.100.255       |255.255.255.0      |172.16.100.1-172.16.100.254|
 
 - le serveur est en 172.16.10.0/24
 
  |adresse      |adresse de réseau |adresse de diffusion | masque sous réseau|plage d'adresses des hotes |
 |:-----------:|:----------------:|:-------------------:|:-----------------:|:--------------------------:|
 |172.16.10.10 |172.16.10.0       |172.16.10.255        |255.255.255.0      |172.16.10.1-172.16.10.254   |

### Q.1.2

- Aller dans la barre de recherche en bas à gauche, tapez Ethernet > cliquer paramètres Ethernet > Centre Réseau et partage > Modifier les paramètres de la carte > Ethernet > Propriétés > Selectionner IPv4 puis Propriétés et changer l'adresse IP.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Change_IPv4.png)

Nous pouvons effectuer un nouveau test pour verifier que la commande ping reussit.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Ping_vers-Serv_OK.png)


### Q.1.3

![]()

le ping fonctionne quand meme, car le client envoie une requete DNS au serveur DNS pour obtenir une adresse ipv4 correspondant au nom de l'hôte.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Ping_vers_Client_apres_desactipv6.png)

### Q.1.4

On voit bien que le client a recupérer une adresse du dhcp a partir de la plage disponible.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Recup_ADD_DHCP.png)

### Q.1.5

le client ne peut pas prendre la premiere adresse afficher de la plage car est l'adresse réseau.

### Q.1.6

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/DHCP.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/DHCP_Reservation.png)

nous allons dans DHCP manage puis clique droit sur reservation et nous entrons l'adresse choisis pour le client 172.16.10.15 et sont adresse mac 08-00-27-73-3B-10. Nous validons et nous pouvons voir que le client a recupéré l'adresse réservé.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex1/Reservation_OK.png)

### Q.1.7

Grace a l'IPv6 nous avons un espace d'adresses étendu car les adresses IPv6 sont en 128bits et les IPv4 sont en 32bits . 
IPv6 permet aux appareils de configurer automatiquement leur adresse IP sans l'intervention d'un serveur DHCP.

### Q.1.8

Non, car dans un premier temps la majorité des entreprises travaillent encore en IPv4 et de plus il existe le DHCP pour l'IPv6.
