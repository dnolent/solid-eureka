# Feedback 1

Bonjour Apprenant1,

Après consultation de ton rendu, voici les différents retours applicables à celui-ci. La liste n’étant pas exhaustive :)

## Accessibilité de l’URL

L’URL */signin* n’est pas accessible

## Models

Il serait pertinent de spécifier les types des variables, soit :
- Dans un commentaire situé au-dessus de la variable (PHPDoc)
- Directement dans le type de la variable à partir de **PHP 7.4**

### Classe AppUser

Il manque l’insertion, la mise à jour et la suppression d’un utilisateur.
Les méthodes "insert" et "update" devraient être déclarées (en spécifiant la visibilité : "*protected*").

#### Classes Student et Teacher

Il n’est pas toujours nécessaire d’envelopper les variables dans des accolades (ligne 97 de la classe Student par exemple).
```
{$this->firstname} -> $this->firstname
```
Le fait que la variable $sql comportent des guillemets doubles permet à l’interpréteur PHP d’exécuter le contenu de celle-ci et il va « comprendre » qu’il s’agit d’une variable PHP.

Lien vers l'explication : https://www.php.net/manual/fr/language.types.string.php#language.types.string.syntax.double