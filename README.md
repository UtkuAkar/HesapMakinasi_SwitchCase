# HesapMakinasi_SwitchCase
HesapMakinasi_SwitchCase


import  java.util.Scanner;

public class hesapmakinasi {

    public static void main(String[] args) {

        int n1, n2, select;

        Scanner input = new Scanner(System.in);
        System.out.println("1. Sayıyı Giriniz : ");
        n1 = input.nextInt();
        System.out.println("2. Sayıyı Giriniz : ");
        n2 = input.nextInt();

        System.out.println("1-Toplama \n2-Cıkarma \n3-Carpma \n4-Bolme");
        System.out.println("SecımızınIZ nEDIR : ");
        select = input.nextInt();


        switch (select) {
            case 1:
                System.out.println("Toplama : " + (n1 + n2));
                break;
            case 2:
                System.out.println("Cıkarma : " + (n1 - n2));
                break;
            case 3:
                System.out.println("Carpma : " + (n1 * n2));
                break;
            case 4:
                switch (n2) {
                    case 0:
                        System.out.println("Sayı 0 a Bolunemez");
                        break;

                    default:
                        System.out.println("Bolme : " + (n1 / n2));


                }
        }
  }
}
