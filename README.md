# KDV-Tutar-Hesaplayan-Program

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {


     double tutar,kdvOran1=0.18,kdvOran2=0.8,kdvTutar,kdvliTutar;

     Scanner input = new Scanner(System.in);

        System.out.println("Ücret Tutarını Giriniz:  " );

        tutar = input.nextDouble();
        if(tutar<1000) {

            kdvTutar = tutar * kdvOran1;
            kdvliTutar = tutar + kdvTutar;

            System.out.println("KDV'siz tutar: " + tutar);
            System.out.println("KDV Oranı: " + kdvOran1);
            System.out.println("KDV Tutarı : " + kdvTutar);
            System.out.println("KDV li Tutar: " + kdvliTutar);
        }else{
            kdvTutar = tutar * kdvOran2;
            kdvliTutar = tutar + kdvTutar;

            System.out.println("KDV'siz tutar: " + tutar);
            System.out.println("KDV Oranı: " + kdvOran2);
            System.out.println("KDV Tutarı : " + kdvTutar);
            System.out.println("KDV li Tutar: " + kdvliTutar);

        }

        
    }
}
