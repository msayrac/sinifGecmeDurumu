# sinifGecmeDurumu
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        int mat, fizik, turkce, kimya, muzik;
        double average;
        int sayac =0;
        double toplam =0;
        Scanner input = new Scanner(System.in);
        System.out.println("Matematik notunuz : ");
        mat = input.nextInt();
        if(mat>0&&mat<=100){
            sayac++;
            toplam = toplam+mat;
        } else {
            System.out.println("Gecersiz deger");
        }
        System.out.println("Fizik notunuz : ");
        fizik = input.nextInt();
        if(fizik>0&&fizik<=100){
            sayac++;
            toplam = toplam+fizik;
        } else {
            System.out.println("Gecersiz deger");
        }
        System.out.println("TUrkce notunuz : ");
        turkce = input.nextInt();
        if(turkce>0&&turkce<=100){
            sayac++;
            toplam = toplam+turkce;
        } else {
            System.out.println("Gecersiz deger");
        }
        System.out.println("Kimya notunuz : ");
        kimya = input.nextInt();
        if(kimya>0&&kimya<=100){
            sayac++;
            toplam = toplam+kimya;
        } else {
            System.out.println("Gecersiz deger");
        }
        System.out.println("Muzik notunuz : ");
        muzik = input.nextInt();
        if(muzik>0&&muzik<=100){
            sayac++;
            toplam = toplam+muzik;
        } else {
            System.out.println("Gecersiz deger");
        }
        average = (toplam)/sayac;
        System.out.println(average);
        if(average<55){
            System.out.println("Sınıfta kaldınız");
            System.out.println("Ortalamanız : " + average);
        } else {
            System.out.println("Gectiniz");
            System.out.println("Ortalamanız : " + average);
        }
    }
}
