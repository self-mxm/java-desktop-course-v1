# 5. Boucles

`for` convient lorsqu’on compte les répétitions :

```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Tour " + i);
}
```

Les trois parties sont l’initialisation, la condition de continuation et la mise à jour. Vérifiez les bornes et que la mise à jour rapproche de la fin.

`while` teste avant le tour et peut ne jamais s’exécuter :

```java
int compte = 3;
while (compte > 0) {
    System.out.println(compte);
    compte--;
}
```

`do-while` exécute le bloc au moins une fois : `do { essai++; } while (essai < 1);` (notez le point-virgule final).

Une boucle améliorée parcourt directement les éléments :

```java
for (int nombre : nombres) {
    System.out.println(nombre);
}
```

`break` quitte une boucle et `continue` saute au tour suivant. Utilisez-les avec modération. Exercices : affichez 1 à 20, calculez la somme de 1 à 100 et affichez la table d’un nombre.
