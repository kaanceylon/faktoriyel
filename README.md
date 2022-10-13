# faktoriyel
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int n, r, comb, totalr=1, totaln=1, totalnr=1;

        Scanner input = new Scanner(System.in);
        System.out.print( "C(n,r) bicimindeki n degerini giriniz: ");
        n = input.nextInt();
        System.out.print( "C(n,r) bicimindeki r degerini giriniz: ");
        r = input.nextInt();

        for (int i=1; i<=n; i++){
            totaln = totaln * i;
        }
        for (int j=1; j<=r; j++){
            totalr = totalr * j;
        }
        int nFark = n -r ;
        for (int k=1; k<= nFark; k++){
            totalnr = totalnr * k;

        }
        comb = totaln/(totalr*totalnr);
        System.out. print("C(" + n + "," + r + ") = " + comb);







    }
}

































