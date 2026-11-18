# 2. Variables et types

Une variable nommée stocke une valeur. Son type détermine les valeurs possibles.

```java
String prenom = "Amina";
int age = 20;
double taille = 1.68;
boolean estEtudiante = true;
char initiale = 'A';
System.out.println(prenom + " a " + age + " ans.");
```

Types fréquents : `int` pour un entier, `long` pour un entier plus grand (suffixe `L`), `double` pour un décimal, `boolean` pour `true`/`false`, `char` pour un caractère et `String` pour du texte. `String` est une classe, les autres exemples sont des types primitifs.

Une variable peut être réaffectée : `age = age + 1;`. La convention camelCase rend les noms lisibles (`nombreDeTentatives`). Pour une valeur constante, utilisez `final`, par exemple `final double TAUX = 0.18;`.

Une conversion de `int` vers `double` est automatique. Une conversion réductrice doit être explicite : `(int) 3.9` vaut `3` et perd la partie décimale. Les décimaux binaires ne représentent pas toujours précisément les fractions ; les applications financières utilisent souvent `BigDecimal`.

Exercice : déclarez une ville, une température, une population et un booléen indiquant s’il pleut ; affichez une phrase avec ces informations.
