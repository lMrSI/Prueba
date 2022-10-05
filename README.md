import java.util.Scanner;
public class MisTiendas {
    public static void main(String args[]) {
        Scanner a = new Scanner(System.in);
        double tienda1 = Double.parseDouble(args[0]);
        double tienda2 = Double.parseDouble(args[1]);
        double tienda3 = Double.parseDouble(args[2]);
        double tienda4 = Double.parseDouble(args[3]);
        String economico = "";
        if (tienda1 <= tienda2){
            if (tienda2 <= tienda3){
                if (tienda3 <= tienda4){
                    System.out.println(" La tienda mas barata es: " + (economico = economico + tienda1));
                } else {
                    System.out.println(" La tienda mas barata es: " + (economico = economico + tienda2));
                }
            } else {
                System.out.println(" La tienda mas barata es: " + (economico = economico + tienda3));
            }
        } else {
            System.out.println(" La tienda mas barata es: " + (economico = economico + tienda4));
        }
        double descuento = a.nextDouble();
        double precioFinal = Double.parseDouble(economico);
        System.out.println(" El descuento es: " + descuento + "%");
        precioFinal = precioFinal - (precioFinal * descuento / 100);
        System.out.println(" Pagaremos: " + precioFinal);
    }
}
