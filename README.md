# Persamaan-Kuadrat
package persamaankuadrat;
import java.util.Scanner;

public class PersamaanKuadrat {
    public static void main(String[] args) {
       Scanner input = new Scanner (System.in);
       System.out.print("a= ");
       double a = input.nextDouble();
       System.out.print("b= ");
       double b = input.nextDouble();
       System.out.print ("c= ");
       double c = input.nextDouble();
       double d = (b*b)-(4*a*c);
       if (a!=0){
           if (d==0){
               double x = -b/(2*a);
               System.out.println("Kedua akarnya adalah "+x);
           }else if (d>0){
               double x1 = (-b+(Math.sqrt(d)))/2*a;
               System.out.println("x1= "+x1);
               double x2 = (-b-(Math.sqrt(d)))/2*a;
               System.out.println("x2= "+x2);
           }else if (d<0) {
               System.out.println("Kedua akar merupakan bilangan kompleks");
           }
       }
    }
}
