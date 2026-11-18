# 1. Introduction à Java

Java est un langage généraliste, fortement typé et orienté objet. Le compilateur transforme le code source en bytecode ; la machine virtuelle Java (JVM) exécute ce bytecode. Le JDK fournit notamment le compilateur et les outils nécessaires.

Enregistrez l’exemple sous `Bonjour.java` :

```java
public class Bonjour {
    public static void main(String[] args) {
        System.out.println("Bonjour, Java !");
    }
}
```

`class` déclare une classe. Le fichier porte le même nom que la classe publique. `main` est le point d’entrée, et `println` affiche une ligne.

```sh
javac Bonjour.java
java Bonjour
```

Résultat : `Bonjour, Java !`. Java distingue les majuscules des minuscules. Les instructions se terminent généralement par `;` et les accolades délimitent les blocs. `//` introduit un commentaire sur une ligne. Essayez de remplacer le message et comparez `print` avec `println`.
