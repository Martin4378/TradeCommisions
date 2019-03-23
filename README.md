# TradeCommisions

import java.util.Scanner;

public class P29_TradeCommisions {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String town = scanner.nextLine();
        double sales = Double.parseDouble(scanner.nextLine());
        double commision = -1;
        
        double percent1Sofia = 0.05;
        double percent2Sofia = 0.07;
        double percent3Sofia = 0.08;
        double percent4Sofia = 0.12;

        double percent1Varna = 0.045;
        double percent2Varna = 0.075;
        double percent3Varna = 0.1;
        double percent4Varna = 0.13;

        double percent1Plovdiv = 0.055;
        double percent2Plovdiv = 0.08;
        double percent3Plovdiv = 0.12;
        double percent4Plovdiv = 0.145;
        

        if(town.equalsIgnoreCase("sofia")){

            if(sales <= 500 && sales >= 0){
                commision = sales * percent1Sofia;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales <= 1000 && sales > 500) {
                commision = sales * percent2Sofia;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales > 1000 && sales <= 10000) {
                commision = sales * percent3Sofia;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales >= 1000 ) {
                commision = sales * percent4Sofia;
                System.out.printf("%.2f%n" , commision);
            }
            else {
                System.out.println("error");
            }
            
        }
        else if(town.equalsIgnoreCase("varna")){

            if(sales <= 500 && sales >= 0){
                commision = sales * percent1Varna;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales <= 1000 && sales > 500) {
                commision = sales * percent2Varna;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales > 1000 && sales <= 10000) {
                commision = sales * percent3Varna;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales >= 1000 ) {
                commision = sales * percent4Varna;
                System.out.printf("%.2f%n" , commision);
            }
            else {
                System.out.println("error");
            }
            
        }
        else if(town.equalsIgnoreCase("plovdiv")) {

            if(sales <= 500 && sales >= 0){
                commision = sales * percent1Plovdiv;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales <= 1000 && sales > 500) {
                commision = sales * percent2Plovdiv;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales > 1000 && sales <= 10000) {
                commision = sales * percent3Plovdiv;
                System.out.printf("%.2f%n" , commision);
            }
            else if(sales >= 1000 ) {
                commision = sales * percent4Plovdiv;
                System.out.printf("%.2f%n" , commision);
            }

            else {
                System.out.println("error");
            }
            
        }
        else {
            System.out.println("error");
        }




    }
}
