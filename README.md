# Java-primeNumber
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package primenumber;

import java.util.Scanner;

/**
 *
 * @author HP
 */
public class PrimeNumber {

    public static void main(String[] args) {
        int count=0;
        Scanner a = new Scanner(System.in);
        System.out.println("Enter Number ");
       int x = a.nextInt();
        if( x==0 || x==1){
            count++;
        }
        for(int i=2;i<x; i++){
            if(x%i==0){
                count++;
            }
           
        }
        if(count ==0){
               System.out.println(x+" is prime Number");
           }else{
                System.out.println(x+" isn't prime Number");
           }
    }
    
}
