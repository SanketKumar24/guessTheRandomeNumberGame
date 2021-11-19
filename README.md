# guessTheRandomeNumberGameInJava

package com.company;
import java.util.Scanner;
import java.util.Random;

public class RandomNumberGenerator {
    public static void main(String[] args) {
    
        System.out.println("lets see at how maney times you can guess a mumber (0 to 100) :) \n");
        System.out.println("Enter the number");
        Scanner s = new Scanner(System.in);
        Random rand = new Random();
        int a;
        int guess=1;
        int num;
        num =rand.nextInt(101);

        do {
            a = s.nextInt();

            if (num>a){
                System.out.println("too low");
            }
            if (num<a){
                System.out.println("too high");
            }
            if (a==num){
                break;
            }
            guess++;
        }while (true);



        System.out.println("you got in "+guess+" times");

    }
}
