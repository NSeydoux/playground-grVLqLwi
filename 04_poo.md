```java runnable
//{ autofold
import java.util.ArrayList;


public class Main {
//}
    public static class Maison {
        private Integer surface;
        private Integer nombrePieces;
        private String adresse;
        private Boolean jardin;
    
        public Maison(Integer surface, Integer nombrePieces, String adresse, Boolean jardin){
            this.surface = surface;
            this.nombrePieces = nombrePieces;
            this.adresse = adresse;
            this.jardin = jardin;
        }
    
        public Integer getSurface(){
            return this.surface;
        }
    
        public Integer getNombrePieces(){
            return this.nombrePieces;
        }
    
        public void setNombrePieces(Integer pieces){
            if(pieces > 0){
                this.nombrePieces = pieces;
            }
        }
    
        public String getAdresse(){
            return this.adresse;
        }
    
        public Boolean hasJardin(){
            return this.jardin;
        }
    
        public String toString(){
            String result = "Votre maison de "+this.surface+"m², située au "+this.adresse+", a "+this.nombrePieces+" pièces et ";
            if(this.jardin){
                result += " un jardin.";
            } else {
                result += " pas de jardin.";
            }
            return result;
        }
    }

    // Le main est une fonction particulière, c'est elle qui est appelée quand on exécute le programme. 
    public static void main(String[] args) {
        Maison maMaison = new Maison(60, 4, "42, rue du manchot", false);
        System.out.println(maMaison.toString());
        ArrayList<Maison> mesMaisons = new ArrayList<Maison>();
        mesMaisons.add(maMaison);
        for(Maison m : mesMaisons){
            System.out.println(m.toString());
        }
    }
//{ autofold    
}
//}

```

- Créez trois maison différentes
- La mairie décide de renommer les rues ! Faites en sorte de pouvoir changer publiquement les adresses des maisons, et changez les adresses des maisons que vous avez déjà créées.
- Vous voulez maintenant pouvoir attribuer les bureaux inoccupés à l'hébergement d'urgence. Ajoutez une propriété pour déterminer si une maison est un bâtiment personnel ou professionnel, et une autre pour déterminer si la maison est occupée. Vous pouvez maintenant ajouter une méthode indiquant si la maison peut être attribuée à l'hébergement d'urgence.