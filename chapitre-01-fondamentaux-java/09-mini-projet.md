# 9. Mini-projet — Carnet de notes

L’application demande combien de notes seront saisies, les conserve dans un tableau, calcule la moyenne et indique si elle atteint 10.

```java
import java.util.Scanner;

public class CarnetDeNotes {
    public static void main(String[] args) {
        Scanner clavier = new Scanner(System.in);
        System.out.print("Nombre de notes : ");
        int nombre = clavier.nextInt();
        if (nombre <= 0) {
            System.out.println("Le nombre doit être positif.");
            clavier.close();
            return;
        }
        double[] notes = new double[nombre];
        double somme = 0;
        for (int i = 0; i < notes.length; i++) {
            System.out.print("Note " + (i + 1) + " : ");
            notes[i] = clavier.nextDouble();
            somme += notes[i];
        }
        double moyenne = somme / notes.length;
        System.out.printf("Moyenne : %.2f%n", moyenne);
        System.out.println(moyenne >= 10 ? "Moyenne atteinte." : "Moyenne non atteinte.");
        clavier.close();
    }
}
```

Enregistrez sous `CarnetDeNotes.java`. `%.2f` affiche deux décimales. La vérification du nombre empêche une division par zéro.

Améliorations : refusez les notes hors de 0–20 ; affichez minimum, maximum et nombre de notes validées ; déplacez le calcul dans une méthode `calculerMoyenne(double[] notes)`. Testez zéro note, une seule note et des valeurs aux limites.
