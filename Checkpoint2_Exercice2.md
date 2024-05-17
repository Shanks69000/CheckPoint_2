### Q.2.1
Créer un dossier partage a la racine C: quon colle le dossier script dedans.

Pour partager un dossier il va falloir aller dans le gestionnaire de serveur, installer les roles share.

Puis aller dans **File and storage services** , ensuite cliquer sur la petites etiquette **tasks**.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/storage_service.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/share.png)

Selectionner le **partage rapide**, choisir le chemin et le dossier partage suivre les indications et laisser les configue par defaut.

puis créer.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/conf_share.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/conf_share_2.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/conf_share_3.png)


Maintenant aller sur le client dans la barre de recherche taper **\\176.16.10.10\Partage** cliquer sur le fichier afficher.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/entrer_ip.png)

Rentrer les identifiants administrateur, puis copier coller le fichier scripts dans la racine C: du client.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/entrer_acces.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/dossier_partager.png)

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/coller_dossier.png)

## Q.2.2

Rien ne se passe a l'execution du script une fenêtre s'ouvre et se referme.

### Q.2.3
-Verb RunAs : Permet d'exécuter le script avec des privilèges administratifs.

### Q.2.4
-WindowsStyle Maximized : Lance la fenêtre PowerShell en mode maximisé.

### Q.2.5

A la ligne 27 du fichier addLocalUser.ps1 il y a la methode select-object **-skip 2**, nous pouvons le supprimé pour enlever se problème.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20120422.png)

### Q.2.6

A la ligne 38 $Description n'etais pas ajouté à $UserInfo donc c'est pour cela que le script ne l'affiche pas.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20120904.png)

### Q.2.7

A la ligne 27 il manque  $Users le select-Object avec ce quon desire récupérer dans le fichier csv.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20121434.png)

### Q.2.8

A la ligne 50 on rajoute au Write-Host **-ForegroundColor Green** 

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20121758.png)

### Q.2.9

il y a deux façon : 
-l'appeler directement dans le script

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20123032.png)

- importer le modules fonction.psm1 et appeler la fonction log

### Q.2.10

Il faut enlever le !not a la ligne 34 et ajouter un Write-Host puis rajouter un else pour enchainer la suite.

![](https://github.com/Shanks69000/CheckPoint_2/blob/main/img_ex2/Capture%20d'%C3%A9cran%202024-05-17%20122651.png)

### Q.2.11

### Q.2.12

### Q.2.13

### Q.2.14

### Q.2.15
