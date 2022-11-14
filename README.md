# Daire_diliminin_alani
Yarıçapı r, merkez açısının ölçüsü 𝛼 olan daire diliminin alanı bulan programı yazınız.

import java.text.DecimalFormat;

import java.util.Scanner;

public class daire_dilimi {

    public static void main(String[] args){
    
        Scanner input= new Scanner(System.in);

        System.out.println("dairenin yarıçapını girin: ");
        int r= input.nextInt();
        System.out.println("dairenin merkez açı ölçüsünü girin: ");
        int a= input.nextInt();
        double pi=3.14;

        double alan= (pi*(r*r)*a)/360;
        DecimalFormat df=new DecimalFormat("##.##");
        alan=Double.valueOf(alan);
        System.out.println("daire diliminin alanı: " +df.format(alan));

    }
}
