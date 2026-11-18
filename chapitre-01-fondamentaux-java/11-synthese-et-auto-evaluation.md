# 11. Synthèse et auto-évaluation

## À retenir

- Le JDK compile le code source ; la JVM exécute le bytecode.
- `main` est le point d’entrée conventionnel d’un programme Java.
- Chaque variable a un type ; `String` contient du texte et les types primitifs courants incluent `int`, `double` et `boolean`.
- Les comparaisons produisent des booléens ; utilisez `equals` pour comparer le contenu de chaînes.
- `if` et `switch` choisissent ; `for`, `while` et `do-while` répètent.
- Une méthode nomme une opération, prend éventuellement des paramètres et retourne éventuellement une valeur.
- Les tableaux ont une taille fixe ; leurs indices vont de zéro à `length - 1`.
- Après `nextInt()`, consommez le retour à la ligne avant d’appeler `nextLine()`.

## Questions

1. Quelle différence entre compiler et exécuter ?
2. Que vaut `7 / 2` si les deux opérandes sont des `int` ? Comment obtenir un décimal ?
3. Pourquoi préférer `equals` à `==` pour deux chaînes ?
4. Quel est le dernier indice d’un tableau de longueur 6 ?
5. Comment éviter une division par zéro dans une moyenne ?

## Réponses

1. La compilation produit le bytecode ; l’exécution lance le programme sur la JVM.
2. `3` ; convertissez un opérande en `double`, par exemple `7.0 / 2`.
3. `==` compare les références ; `equals` compare le contenu.
4. `5`.
5. Vérifiez que le tableau contient au moins une valeur.

Vous êtes prêt à poursuivre si vous pouvez écrire un petit programme console, le décomposer en étapes, choisir des types, utiliser une condition et une boucle et vérifier les cas limites. Reprenez une leçon si vous ne pouvez pas encore expliquer ses exemples.
