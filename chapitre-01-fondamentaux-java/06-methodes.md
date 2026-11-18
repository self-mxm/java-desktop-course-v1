# 6. Méthodes

Une méthode regroupe une opération réutilisable. Elle peut recevoir des paramètres et retourner une valeur.

```java
public class Calculatrice {
    static int additionner(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        System.out.println(additionner(7, 5));
    }
}
```

`int` indique le type retourné. `return` renvoie le résultat et termine la méthode. Ici, les méthodes sont `static` pour être appelées directement depuis `main`, qui est statique ; les méthodes d’instance viendront plus tard.

Une méthode sans résultat utilise `void`, par exemple `static void saluer(String prenom)`. Les variables locales ne sont accessibles que dans leur méthode. Une surcharge permet plusieurs méthodes du même nom si leurs paramètres diffèrent ; le type de retour seul ne suffit pas.

Choisissez un nom clair et une seule responsabilité par méthode. Exercices : écrivez `estPair(int n)`, `convertirEnMinutes(int heures, int minutes)` et `afficherTable(int n)`.
