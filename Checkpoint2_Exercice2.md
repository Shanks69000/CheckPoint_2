### Q.2.1
Créer un dossier partage a la racine C: quon colle le dossier script dedans.

Pour partager un dossier il va falloir aller dans le gestionnaire de serveur, installer les roles share.

Puis aller dans **File and storage services** , ensuite cliquer sur la petites etiquette **tasks**.

Selectionner le **partage rapide**, choisir le chemin et le dossier partage suivre les indications et laisser les configue par defaut.

puis créer.

Maintenant aller sur le client dans la barre de recherche taper **\\176.16.10.10\Partage** cliquer sur le fichier afficher.

Rentrer les identifiants administrateur, puis copier coller le fichier scripts dans la racine C: du client.

## Q.2.2

Rien ne se passe a l'execution du script une fenêtre s'ouvre et se referme.

### Q.2.3
-Verb RunAs : Permet d'exécuter le script avec des privilèges administratifs.

### Q.2.4
-WindowsStyle Maximized : Lance la fenêtre PowerShell en mode maximisé.

### Q.2.5

A la ligne 27 du fichier addLocalUser.ps1 il y a la methode select-object **-skip 2**, nous pouvons le supprimé pour enlever se problème.

### Q.2.6

A la ligne 38 $Description n'etais pas ajouté à $UserInfo donc c'est pour cela que le script ne l'affiche pas.

### Q.2.7

A la ligne 27 il manque  $Users le select-Object avec ce quon desire récupérer dans le fichier csv.

### Q.2.8

A la ligne 50 on rajoute au Write-Host **-ForegroundColor Green** 

### Q.2.9

il y a deux façon : 
-l'appeler directement dans le script
- importer le modules fonction.psm1 et appeler la fonction log

### Q.2.10

Il faut enlever le !not a la ligne 34 et ajouter un Write-Host puis rajouter un else pour enchainer la suite.

### Q.2.11