### 1. Programmation Fonctionnelle

**Définition :** La programmation fonctionnelle est un paradigme de programmation où les programmes sont construits en appliquant et en composant des fonctions. Elle met l'accent sur les fonctions sans effets secondaires et l'immutabilité des données.

**Exemple :** En Haskell, un exemple simple serait une fonction pour calculer la somme d'une liste :

```haskell
sommeListe :: [Int] -> Int
sommeListe = foldr (+) 0

main = print (sommeListe [1, 2, 3, 4, 5])
```

### 2. Programmation Impérative

**Définition :** La programmation impérative est basée sur le concept de déclarations d'instructions qui changent l'état d'un programme. Elle est centrée sur la description des étapes que l'ordinateur doit suivre pour atteindre un état désiré.

**Exemple :** En C, modifier la valeur d'une variable :

```c
#include <stdio.h>

int main() {
    int a = 5;
    a = a + 1; // Modification de l'état de la variable 'a'
    printf("%d\n", a);
    return 0;
}
```

### 3. Programmation Déclarative

**Définition :** Contrairement à la programmation impérative, la programmation déclarative se concentre sur ce que doit accomplir le programme, plutôt que sur comment il doit le faire. SQL et HTML sont des exemples de langages déclaratifs.

**Exemple :** En SQL, récupérer les noms des employés :

```sql
SELECT nom FROM employes;
```

### 4. Programmation Logique

**Définition :** La programmation logique est basée sur la logique formelle. Le programme est un ensemble de faits et de règles qui décrivent des relations. Prolog est un exemple de langage de programmation logique.

**Exemple :** En Prolog, vérifier si une personne est parent d'une autre :

```prolog
parent(alice, bob).

estParent(X, Y) :- parent(X, Y).
```

### 5. Programmation Par Contraintes

**Définition :** La programmation par contraintes spécifie les relations entre les variables en termes de contraintes et cherche des solutions qui les satisfont. Elle est souvent utilisée en planification, en affectation de ressources et en résolution de puzzles.

**Exemple :** Trouver des valeurs de X et Y telles que X + Y = 10 et X - Y = 4.

Ce problème peut être résolu par un solveur de contraintes sans qu'il soit nécessaire d'écrire explicitement comment trouver X et Y.

### 6. Programmation Réactive

**Définition :** La programmation réactive est orientée autour de la gestion des flux de données et de la propagation du changement. Elle est particulièrement utile dans les applications avec des interfaces utilisateur interactives et dans le développement de systèmes en temps réel.

**Exemple :** Dans RxJS (une bibliothèque de programmation réactive pour JavaScript), créer un flux de données qui émet une valeur toutes les secondes :

```javascript
const { interval } = require('rxjs');
const observable = interval(1000);
observable.subscribe(x => console.log(x));
```
