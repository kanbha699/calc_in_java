# calc_in_java
 import java.util.Scanner;

import javax.imageio.plugins.tiff.ExifTIFFTagSet;

public class Calc {

    public static void sum(){
        int n;
        System.out.println("how many number u want to sum");
        Scanner sc = new Scanner(System.in);
        n= sc.nextInt();
        int []arr = new int[n];
        for (int i = 0; i < n; i++) {
            System.out.println("enter the " + i + " number");
            arr[i]=sc.nextInt();
        }

        int sum = 0;
        for (int i = 0; i < n; i++) {
        sum =  sum + arr[i];
        }
        System.out.println();
System.out.println("********************************************************************");
System.out.println();
        System.out.println("Your sum " + sum);
        System.out.println();
        System.out.println("********************************************************************");

    }//end of sum function 


    //************************************************************************************************************* */

    public static void substract(){
        int n;
        System.out.println("how many number u want to subtrac ");
        Scanner sc = new Scanner(System.in);
        n= sc.nextInt();
        int sum = 0;
        for (int i = 1; i <= n; i++) {
            int k;
            System.out.print("Enter number " + i + ": ");
            k=sc.nextInt();
            sum -= k;
        }
        System.out.println("The result of subtraction is " + sum);
        

    }//ene of subtractor

//********************************************************************************************************** */
//                                                      division
//********************************************************************************************************** */
public static void division(){
    int a,b;
    Scanner sc = new Scanner(System.in);
    System.out.println("enter a");
    a=sc.nextInt();
    System.out.println("enter b");
    b=sc.nextInt();

    int c = a / b;

    System.out.println("your division:-\t" +c);

    System.out.println("your modulo is " +a%b);

} //end of division
//********************************************************************************************************** */ */
//                                                   multiplication
//************************************************************************************************************ */
public static void multiplication(){
    int n;
    System.out.println("how many numebr of multipicstion you want");
    Scanner sc = new Scanner(System.in);
    n=sc.nextInt();

    int mun=1;

    for (int i = 1; i <= n; i++) {
        int k;
        System.out.println("enter " + i + " number");
        k=sc.nextInt();

        mun = mun*k;
    }
    System.out.println("your multiplication is :-\t" +mun+ "\t<------------");
}//end of multiplication


    public static void main(String[] args) {
        // make a calsator using java 

        System.out.println();
        System.out.println("********************************************************************************************************");

        System.out.println("                            Your claculator");

        System.out.println();
        System.out.println("**********************************************************************************************************");

        System.out.println();
        System.out.println();

        System.out.println("                            what you want to do ");

        System.out.println();
        System.out.println();
        int chois;
        Scanner sc = new Scanner(System.in);
        System.out.println();
        System.out.println();
        System.out.println("$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$");
        System.out.println("$                                                                       $");
        System.out.println("$                   press eny to continue                               $");
        System.out.println("$                                                                       $");
        System.out.println("$                   for exit press 0                                    $");
        System.out.println("$                                                                       $");
        System.out.println("$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$");
        chois= sc.nextInt();
        while (chois !=0) {
        System.out.println("\t\t\t******************************************************************");
        System.out.println("\t\t\t*           1->Sum                                               *");
        System.out.println("\t\t\t*           2->Subtraction                                       *");
        System.out.println("\t\t\t*           3->Multipliction                                     *");
        System.out.println("\t\t\t*           4->Division                                          *");
        System.out.println("\t\t\t*           5-> exits                                            *");
        System.out.println("\t\t\t******************************************************************");

            int i;
            System.out.println("enter");
            i=sc.nextInt();
        
        switch(i){
            case 1:
            sum();
            break;

            case 2:
            substract();
            break;

            case 3:
            multiplication();
            break;

            case 4:
            division();
            break;

            case 5:
            chois = 0;
            break;

            default:
            System.out.println("not  valid chois ");
            break;
        }
        
    }
        


    System.out.println("K@nbh@");
    }
    
}

