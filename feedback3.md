#Feedback 3

Bonjour Apprenant3,

Après consultation de ton rendu, voici les différents retours applicables à celui-ci. La liste n’étant pas exhaustive :)

## Controllers

### Classe MainController

Entre la déclaration du namespace et celle de la classe, il n’est pas nécessaire de laisser plusieurs lignes vides.
La classe devrait hériter d’une classe CoreController.

Ligne 14 il serait utile de préciser le type du deuxième paramètre de la méthode.

### Classe CoreController

La classe CoreController est absente.

### Classe TeacherController

À la ligne 35, l’objet $newStudent n’est pas utilisable directement car il faut d’abord réaliser l’instanciation de celui-ci.

## Models

Il est possible de déclarer le type d’une variable directement dans le code à partir de PHP 7.4
```
public int $id;
```

### Classe Student

Il n’est pas toujours nécessaire d’envelopper les variables dans des accolades (ligne 35 de la classe Student par exemple).
```
{$this->firstname} -> $this->firstname
```
Le fait que la variable $sql comportent des guillemets doubles permet à l’interpréteur PHP d’exécuter le contenu
de celle-ci et il va "comprendre" qu’il s’agit d’une variable PHP.

L’utilisation de *var_dump* dans le code est à proscrire, il y a d’autres façons d’afficher les erreurs à l’utilisateur.
L’utilisation de la fonction var_dump doit servir uniquement pour le déboggage,
il faut absolument bannir son utilisation dans un environnement de production.

Attention aux nombreux sauts de lignes inutiles dans le code, entre les méthodes par exemple.