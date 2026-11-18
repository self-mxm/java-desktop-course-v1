# 8. Saisie utilisateur

`Scanner` lit la console. Enregistrez et exécutez ce programme :

```java
import java.util.Scanner;

public class Saisie {
    public static void main(String[] args) {
        Scanner clavier = new Scanner(System.in);
        System.out.print("Votre prénom : ");
        String prenom = clavier.nextLine();
        System.out.print("Votre âge : ");
        int age = clavier.nextInt();
        System.out.println("Bonjour " + prenom + ", vous avez " + age + " ans.");
        clavier.close();
    }
}
```

`nextLine()` lit une ligne entière, `nextInt()` un entier et `nextDouble()` un décimal. Après `nextInt()`, le retour à la ligne reste dans l’entrée ; consommez-le avant un autre `nextLine()` :

```java
int age = clavier.nextInt();
clavier.nextLine(); // consomme le retour à la ligne
String ville = clavier.nextLine();
```

Une entrée incorrecte peut provoquer une exception. Plus tard, vous apprendrez à la gérer ; on peut aussi lire une chaîne puis appeler `Integer.parseInt(texte)`. Fermez le scanner après usage et évitez d’en créer plusieurs sur `System.in`.

Exercice : demandez le prénom et l’année de naissance puis affichez un âge approximatif (l’anniversaire exact n’étant pas connu).
