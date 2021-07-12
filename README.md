# O'Tableau

## Notions travaillées

- Sélecteurs
- Event listeners
- Boucles
- Modification du DOM

## Instructions

On va aider Bart Simpson à écrire ses punitions sur le tableau comme ci-dessous :

![exemple](images/exemple.png)

Dans ce dépôt, tu trouveras une page déjà intégrée avec deux champs : _texte du tableau_ et _nombre de lignes_.
Ton but ici sera de faire en sorte que le texte du premier champ apparaisse dans le tableau noir, et autant de fois que le nombre indiqué dans le second champ.

Les changements doivent se faire en direct. C'est à dire que le tableau se met à jour dès qu'on écrit dans l'un des champs.

## Étapes

Voici quelques pistes pour bien commencer :

1. Comme les changements se font en temps réel, il doivent se déclencher à chaque fois qu'une touche du [clavier est relâchée](https://developer.mozilla.org/en-US/docs/Web/API/Document/keyup_event#addeventlistener_keyup_example). Mais pas n'importe où ! Sur l'un des deux champs uniquement. On va donc poser nos écouteurs dessus.
2. A chaque fois qu'un changement est détecté, on récupère les valeurs contenues dans les deux champs.
3. Il faut penser à sélectionner la zone du tableau dans laquelle on va écrire. C'est la div `.text-board`. D'ailleurs elle est peut-être déjà remplie. Un petit nettoyage sera peut-être nécessaire.
4. Comme il faut afficher le même texte plusieurs fois de suite en se basant sur le nombre indiqué dans le second champ, une [boucle](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Instructions/for) peut être utile.
5. On peut ajouter du html dans un élément avec [innerHTML](https://developer.mozilla.org/fr/docs/Web/API/Element/innertHTML). Pour les sauts de lignes, un `<br>` fera l'affaire !

## BONUS

Pour aller plus loin, tu peux ajouter des champs qui permettent de modifier la taille de la police, l'interlignage ou la couleur de la craie en direct !

Si t'as envie d'aller encore plus loin, tu peux faire un champ qui permet de changer d'image de fond. Pourquoi pas faire un générateur pour toutes tes séries préférées ?
