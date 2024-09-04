# ExtensionPack
Pack d'extension pour VS Code, du département de multimédia du Cégep de Matane.


## Ajout d'une extension
Pour ajouter une extenstion, il faut aller dans le fichier [package.json](https://github.com/LauriFernandez/ExtensionPack/blob/main/package.json). À la suite des autres éléments de l'objet : `"extensionPack"`.

Il faut mettre le publisher.name, pour le trouver il suffit d'aller sur le marketplace et de regarde itemName dans l'url.

![Capture d'écran de l'explorateur de fichier](https://github.com/LauriFernandez/ExtensionPack/blob/main/img_readme/marketplace.png)

## Compiler pour le mettre en .vsix

Dans le dossier, ouvrir un terminal.
Installer vsce en global avec la commande 
```
npm install -g @vscode/vsce
```
Mettre à jour la version dans le fichier [package.json](https://github.com/LauriFernandez/ExtensionPack/blob/main/tim-recommendations/package.json)

Ensuite, il suffit de lancer la commande
```
vsce package
```
Dire oui a toutes les questions
Le fichier .vsix est créé

## importer un fichier .vsix
Aller dans l'onglet Extension de vscode
cliquer sur les trois points à côté de la barre de recherche et choisir importer depuis fichier vsix.

![Capture d'écran du menu vs code](https://github.com/LauriFernandez/ExtensionPack/blob/main/img_readme/importer.png)

Choisir le fichier du pack d'extenstion en .vsix

![Capture d'écran de l'explorateur de fichier](https://github.com/LauriFernandez/ExtensionPack/blob/main/img_readme/selection.png)

