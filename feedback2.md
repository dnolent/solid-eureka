# Feedback 2

Bonjour Apprenant2,

Après consultation de ton rendu, voici les différents retours applicables à celui-ci. La liste n’étant pas exhaustive :)

## Contrôleurs

### Classe CoreController

Pour une meilleure lisibilité et des modifications plus simples et rapides, on pourrait réfléchir à une solution pour
exporter la liste des ACL dans un autre fichier et l’importer ensuite dans la classe.

Afin de pouvoir accéder plus vite à un élément, cela pourrait être intéressant de trier les clés par ordre alphabétique.
Une petite vérification s’impose également pour éviter les doublons dans le tableau (lignes 32-33).

### Classe StudentController

Attention à bien respecter l’indentation dans tous les fichiers pour une meilleure lisibilité (lignes **48, 75**, etc.).

Vérifier si la variable de la ligne **105**, à laquelle on ajoute des données ligne **108**, est bien utilisée dans le code quelque part.
Il est préférable d’utiliser un seul type de casse et de le respecter dans l’intégralité du code,
par exemple avec camelCase en PHP (voir PSR-1), à la ligne 17 *$newstudent* devient alors *$newStudent*.
Cela permet d’améliorer la lisibilité et de gagner du temps lors de la lecture du code, c’est également plus confortable.

## Models

Il est possible de déclarer le type d’une variable directement dans le code à partir de **PHP 7.4**

```
public int $id;
```

### Classes Appuser, Student et Teacher

Il n’est pas toujours nécessaire d’envelopper les variables dans des accolades.
```
{$this->firstname} -> $this->firstname
```
Le fait que la variable $sql comportent des guillemets doubles permet à l’interpréteur PHP d’exécuter le contenu
de celle-ci et il va "comprendre" qu’il s’agit d’une variable PHP.

Lien vers l'explication : https://www.php.net/manual/fr/language.types.string.php#language.types.string.syntax.double