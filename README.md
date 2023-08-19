# MahokuTesters

**Le dépôt dédié aux testeurs de Mahoku**, il vous permet de nous signaler les problèmes que vous rencontrez en jeu.

## Guide pour un rapport de bug parfait

Un bug est un _problème démontrable_ causé par le code du jeu ou l'intéraction de l'utilisateur avec celui-ci.
De bons rapports de bugs sont extrêmement utiles - merci ! 🙏

### Lignes directrices pour les rapports de bugs :

1. **Utilisez la recherche de problèmes GitHub** &mdash; vérifiez \[[ici](https://github.com/Nyfos/MahokuTesters/issues?q=is:issue 'Liste des issues')\] si le problème a déjà été
    signalé.

2. **Vérifiez si le problème a été résolu** &mdash; essayez de le reproduire en utilisant la dernière version de développement à laquelle vous avez accès et regadez \[[ici](https://github.com/Nyfos/MahokuTesters/issues?q=is:open+label:"Statut:%20à%20tester","Statut:%20résolu" 'Liste des issues - à tester & résolus')\].

3. **Isolez le problème** &mdash; réduisez au minimum le nombre d'étapes nécessaires pour reproduire le problème, et ciblez la nature de celui-ci.

<br/>

Un bon rapport de bug ne devrait pas obliger les autres à revenir auprès de vous pour obtenir plus d'informations.

Veuillez essayer de détailler autant que possible votre rapport. Quelle machine utilisez-vous et avec quels paramètres ?
Quelles étapes permettront de reproduire le bug ?
Avec quel système d'exploitation rencontrez-vous le problème ?
À quel résultat vous attendiez-vous ?
Tous ces petits détails aideront d'avantage les développeurs à corriger les bugs potentiels.

### Exemple :

> Exemple de titre de rapport de bug court et descriptif
>
> Un résumé du problème et de l'environnement du système d'exploitation dans lequel il se produit.
> Si approprié, incluez les étapes nécessaires pour reproduire le bug.
>
> 1. C'est la première étape ;
> 2. C'est l'étape numéro deux ;
> 3. Étapes trois, etc.
>
> `<pièce-jointe>` - une capture d'écran, une vidéo du problème
>
> Toute autre information que vous souhaitez partager et qui est pertinente pour le problème
> signalé. Cela peut inclure les lignes de code que vous avez identifiées comme étant
> à l'origine du bug, et les solutions potentielles à ce bug (ainsi que vos avis sur leur
> mérite).

### Quelle gravité appliquer pour mon signalement de bug ?

Si vous hésitez lors du choix de la gravité du bug trouvé, n'hésitez pas à vous servir de ce tableau comme référence :

| Gravité | Description | Exemples |
| :--- | :--- | :--- |
| Blocage | Empêche la poursuite des tests lorsque le jeu plante à cause d'un bug | Le jeu se ferme lorsqu'on complète la première quête |
| Critique | Concerne la sécurité du jeu et conduit à l'arrêt d'un programme, à la perte de données, ou à tout autre dommage important. De tels bugs nuisent aux fonctionnalités principales de l'application et sont résolus en priorité | La sauvegarde n'enregistre pas les quêtes du joueur |
| Majeure | Affecte négativement une grande partie du jeu que l'on est en train de tester | Dans la traduction du jeu en englais, du texte n'est pas affiché, il y a des omissions systématiques d'espaces, du texte dépassant les limites de l'écran, du texte non traduit, etc. |
| Mineure | N'influence ni les fonctions de base de l'application ni le processus de test | (Hors traduction) Le texte ne tient pas dans une barre séparée, il y a une césure incorrecte, un espace manquant à un endroit particulier, etc. |
| Banale | A peu d'impact sur le fonctionnement du jeu. On trouve généralement ce type de bug au cours des tests d'interface utilisateur | Mauvaise taille d'un bouton, couleur trop vive d'un objet, etc. |

### Où trouver mon fichier de logs et comment l'ajouter à mon signalement ?

Voici l'emplacement du fichier de logs pour chaque système d'exploitation:

Utilisez la combinaison de touches de la colonne "Raccourci" puis entrez l'emplacement du fichier de logs. Appuyez ensuite sur Entrée ou OK pour accéder au dossier contenant le fichier de logs.

| Système d'exploitation | Emplacement | Nom du fichier | Raccourci |
| :--- | :--- | :--- | :--- |
| Windows | `%AppData%\LocalLow\Mahoku\Mahoku\` | `Player.log` | <kbd>⊞ Win</kbd> + <kbd>R</kbd> |
| Plateformes Universelles Windows (UWP) | `%USERPROFILE%\AppData\Local\Packages\Mahoku\TempState\` | `UnityPlayer.log` | <kbd>⊞ Win</kbd> + <kbd>R</kbd> |
| Linux | `~/.config/unity3d/Mahoku/Mahoku/` | `Player.log` | <kbd>Ctrl</kbd> + <kbd>F10</kbd> <kbd>E</kbd> |
| MacOS | `~/Library/Logs/Mahoku/Mahoku/` | `Player.log` | - |

Lorsque vous envoyez votre signalement, une zone de texte située à la fin de votre signalement vous permet d'ajouter un fichier de logs.
Cliquez sur cette zone pour la mettre en surbrillance puis glissez-y simplement le fichier pour l'ajouter à votre signalement.

## Demandes d'ajout de nouvelles fonctionnalités

Les demandes d'ajout de fonctionnalités sont les bienvenues.
**Mais** prenez un moment pour savoir si votre idée correspond à la portée et aux objectifs du projet.
C'est à *vous* de faire en sorte de convaincre les développeurs du projet du bien-fondé de cette fonctionnalité.
Veuillez fournir autant de détails et de contexte que possible.
