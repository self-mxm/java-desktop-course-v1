# 3. Opérateurs

Les opérateurs calculent ou comparent des valeurs.

```java
int a = 17, b = 5;
System.out.println(a + b); // 22
System.out.println(a / b); // 3 : division entière
System.out.println(a % b); // 2 : reste
System.out.println((double) a / b); // 3.4
```

Les autres opérateurs arithmétiques sont `-` et `*`. `+=` met à jour une variable (`score += 10`), `++` l’incrémente de 1.

Les comparaisons `==`, `!=`, `<`, `<=`, `>` et `>=` produisent un booléen. `&&` signifie ET, `||` OU et `!` NON. `&&` et `||` sont court-circuités : la partie droite peut ne pas être évaluée.

Pour comparer le contenu de chaînes, utilisez `equals` : `reponse.equals("oui")`. `==` compare les références des objets, pas généralement leur contenu. Les parenthèses rendent la priorité explicite : `(2 + 3) * 4` vaut `20`.

Exercices : trouvez quotient et reste de 29 / 6 ; calculez un prix TTC ; créez une condition qui exige une note d’au moins 10 et la présence de l’élève.
