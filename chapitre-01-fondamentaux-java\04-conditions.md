# 4. Conditions

`if` exécute un bloc si sa condition est vraie. Les branches `else if` sont vérifiées dans l’ordre ; `else` couvre les autres cas.

```java
int note = 14;
if (note >= 16) {
    System.out.println("Très bien");
} else if (note >= 10) {
    System.out.println("Réussi");
} else {
    System.out.println("À retravailler");
}
```

Testez les cas limites, comme 9, 10, 15 et 16. Placez les seuils les plus élevés en premier afin qu’une condition générale ne masque pas les autres.

Pour choisir parmi des valeurs discrètes, `switch` est pratique :

```java
int jour = 3;
switch (jour) {
    case 1 -> System.out.println("Lundi");
    case 2 -> System.out.println("Mardi");
    case 3 -> System.out.println("Mercredi");
    default -> System.out.println("Jour inconnu");
}
```

Une expression courte peut utiliser le ternaire : `String statut = age >= 18 ? "majeur" : "mineur";`. Pour une logique complexe, préférez `if`.

Erreur courante : confondre `=` (affectation) et `==` (égalité). Exercice : classez un nombre en positif, négatif ou nul, puis testez zéro.
