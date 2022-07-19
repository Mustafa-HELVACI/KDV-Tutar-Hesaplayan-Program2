# KDV-Tutar-Hesaplayan-Program2
Patika.dev KDV Tutarı Hesaplayan Program

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        //Değişkenleri Oluştur.
        double tutar, kdvOran, kdvliTutar,total ;

        //Kullanicidan Verileri Al
        Scanner input = new Scanner(System.in);
        System.out.print("Ücret Tutarini Girin : ");
        tutar = input.nextDouble();
        
        //Bu Ödevde if ve else kullanmayın denilmediği için if ve else kullandım.
        if(1000 > tutar && tutar < 1000){
            kdvOran=0.08;
        }
        else{
            kdvOran=0.18;
        }

        System.out.println( "Girilen Tutar :" + tutar);
        kdvliTutar = tutar * kdvOran;
        System.out.println("KDV Tutarı :" + kdvliTutar);
        total = tutar + kdvliTutar;
        System.out.println("KDV Dahil Tutar :" + total);


    }
}
