# 7. Tableaux

Un tableau conserve plusieurs valeurs du même type dans une séquence de taille fixe. Les indices commencent à zéro.

```java
int[] notes = {12, 15, 9};
System.out.println(notes[0]); // 12
System.out.println(notes.length); // 3
```

`new int[4]` crée un tableau de quatre entiers initialisés à zéro. Les indices valides vont de 0 à `length - 1` ; dépasser ces bornes déclenche `ArrayIndexOutOfBoundsException`.

```java
int somme = 0;
for (int i = 0; i < notes.length; i++) {
    somme += notes[i];
}
double moyenne = (double) somme / notes.length;
```

Vérifiez que le tableau n’est pas vide avant de calculer une moyenne. Si l’indice n’est pas utile, utilisez `for (int note : notes)`. Un tableau ne peut pas changer de taille ; `ArrayList` sera étudié plus tard.

Exercices : trouvez le maximum d’un tableau non vide ; comptez les notes supérieures ou égales à 10 ; affichez cinq prénoms avec une numérotation commençant à 1.
