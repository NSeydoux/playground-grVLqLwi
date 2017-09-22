# Expressions booléennes

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

Boolean ilPleut= false;
Boolean ilFaitFroid = false;

//Premier IF
if(!ilPleut && !ilFaitFroid){
  System.out.println("HELLO!");
}

//Deuxième IF
if (!(ilPleut || ilFaitFroid)){
  System.out.println("Hello 2 ! ");
}

//{ autofold
}

}
//}
```
En considérant le programme précédent : 

?[Comment exprimer qu'il fait chaud ?]
-[X] !(ilFaitFroid)
-[ ] ilFaitFroid || false

?[Comment exprimer qu'il fait froid et qu'il pleut ? ]
-[ ] ilFaitFroid || ilPleut
-[X] ilFaitFroid && ilPleut

?[Que veut dire la condition dans le premier if ?]
-[X] Il fait beau et il fait chaud
-[X] Il ne pleut pas et il ne fait pas froid

?[Que veut dire la condition dans le deuxième if ?]
-[X] Il fait beau et il fait chaud
-[ ] Il fait froid ou il ne pleut pas
-[ ] Il fait chaud ou il pleut
-[ ] Il fait froid et il pleut
-[ ] Il fait chaud ou il ne pleut pas

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

Integer age = 5;
Boolean permissionDesParents = false;
Boolean droitDeBoire=false;

// Copiez-collez les if ici

System.out.println(droitDeBoire);

//{ autofold
}

}
//}
```

?[Comment écrire qu'il faut la permission des parents ou bien avoir au moins 18 ans pour boire ?]
-[ ] if (permissionDesParents && age >= 18) {droitDeBoire = true;}
-[X] if (permissionDesParents || age >= 18) {droitDeBoire = true;}
-[X] if (permissionDesParents || !(age < 18)) {droitDeBoire = true;}
-[X] if ((permissionDesParents && (age < 18)) || (age >= 18)) {droitDeBoire = true;}
-[ ] if (!permissionDesParents || !(age > 18)) {droitDeBoire = true;}

Pour vous en convaincre, copiez-collez les lignes de la question en dessous du commentaire.


