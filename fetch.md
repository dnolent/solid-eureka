# Fetch (JS)

## Explications

Le langage JavaScript dispose de difféntes API dont l'API Fetch qui permet de fournir une interface permettant d'accéder
à des éléments du protocole HTTP et de les utiliser directement.

Il est possible de trouver un comportement similaire avec XMLHttpRequest qui était utilisé il y a certain nombre d'années.

## Utilisation

Pour utiliser l'API Fetch, il faut que le navigateur qui exécute JavaScript soit compatible.

Il est possible de vérifier sa prise en charge très facilement en exécutant ce code :

```
if (window.fetch) {
  window.alert('Pris en charge !');
} else {
  window.alert('Non pris en charge !');
}
```

