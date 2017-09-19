# Identifiants et typage

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

String messageAAfficher = "Hello World!";
Integer anneeEnCours = 2017;
System.out.println(messageAAfficher);
//System.out.println(anneeEnCours);
Double pi = 3.1415;
anneeEnCours = 2018;
//System.out.println(anneeEnCours);
//{ autofold
}

}
//}
```
En considérant le programme précédent : 

?[Les identifiants son écrits en...]
-[X] Camel case
-[ ] Snake case

?[Les variables messageAAfficher et anneeEnCours sont du même type]
-[ ] Vrai
-[X] Faux

?[Au moment où le message s'affiche, la variable anneeEnCours vaut...]
-[X] 2017
-[ ] 2018

?[À la fin du programme, la variable anneeEnCours vaut...]
-[ ] 2017
-[X] 2018

Pour vous convaincre de ces réponses, vous pouvez effacer les // au début des lignes pour afficher les valeurs.

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

Integer a = 5;
Integer b = 2;
a = 3;
Integer c = a + b;
Boolean aIsGreater = a > b;

//{ autofold
}

}
//}
```

?[À la fin du programme, quelle sera la valeur de c ?]
-[ ] 2
-[ ] 3
-[X] 5
-[ ] 7
-[ ] 8

?[À la fin du programme, quelle sera la valeur de aIsGreater ?]
-[X] Vrai
-[ ] Faux


