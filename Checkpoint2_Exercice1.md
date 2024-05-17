### Q.1.1

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

Nous pouvons effectuer un nouveau test pour verifier que la commande ping reussit.

### Q.1.3

le ping fonctionne quand meme, car le client envoie une requete DNS au serveur DNS pour obtenir une adresse ipv4 correspondant au nom de l'hôte.

### Q.1.4

On voit bien que le client a recupérer une adresse du dhcp a partir de la plage disponible.

### Q.1.5

le client ne peut pas prendre la premiere adresse afficher de la plage car est l'adresse réseau.

### Q.1.6

nous allons dans DHCP manage puis clique droit sur reservation et nous entrons l'adresse choisis pour le client 172.16.10.15 et sont adresse mac 08-00-27-73-3B-10. Nous validons et nous pouvons voir que le client a recupéré l'adresse réservé.

### Q.1.7

Grace a l'IPv6 nous avons un espace d'adresses étendu car les adresses IPv6 sont en 128bits et les IPv4 sont en 32bits . 
IPv6 permet aux appareils de configurer automatiquement leur adresse IP sans l'intervention d'un serveur DHCP.

### Q.1.8

Non, car dans un premier temps la majorité des entreprises travaillent encore en IPv4 et de plus il existe le DHCP pour l'IPv6.