# hesapMakinesiSwitchCase
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int n1, n2, select;
        Scanner inp = new Scanner(System.in);

        System.out.println("Lütfen Birinci Sayıyı Giriniz: ");
        n1 = inp.nextInt();
        System.out.println("Lütfen İkinci Sayıyı Giriniz: ");
        n2 = inp.nextInt();
        System.out.println("Lütfen Yapmak İstediğiniz İşlemi Seçiniz: ");
        System.out.println("Toplama:1 ");
        System.out.println("Çıkartma:2 ");
        System.out.println("Çarpma:3 ");
        System.out.println ("Bölme:4 ");

        select = inp.nextInt();


        switch (select) {
            case 1:
                System.out.print("İşlem Sonucu: " + (n1 + n2));
                break;
            case 2:
                System.out.print("İşlem Sonucu: " + (n1 - n2));
                break;
            case 3:
                System.out.print("İşlem Sonucu: " + (n1 * n2));
                break;
            case 4:
                System.out.println((n2==0 ? "Bir Sayı Sıfıra Bölünemez":"İşlem Sonucu: " +(n1/n2)));
                break;
            default:
                System.out.print("Hatalı Seçim Yaptınız.Tekrar İşlem Seçiniz!!!: ");
                break;
        }
    }
}
