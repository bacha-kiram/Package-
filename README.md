# Package-
Package of homework
package dz.univeloued.tps.classes;

public class Personne {
    private int id;
    protected String nom;
    protected String prenom;
    private static int count = 0;

    public Personne(int id, String nom, String prenom) {
        this.id = id;
        this.nom = nom;
        this.prenom = prenom;
        count++;
    }

    public static int getCount() {
        return count;
    }

    @Override
    public String toString() {
        return "Je suis " + nom + " " + prenom;
    }
}
