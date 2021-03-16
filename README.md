# sesi-3
package com.company;

import java.util.Scanner;
import java.util.Random;

public class Main
{
    public static void main(String[] args)
    {
        Random a = new Random();
        int random1 = a.nextInt(100);
        int x;

        Scanner put = new Scanner(System.in);

        System.out.println("Guess magic number between 0 and 100 \n");

        do {
            System.out.print("Enter your guess: \n");
            x = put.nextInt();

            if(x > random1){
                System.out.println("Your guess is too high");
            } else if (x < random1) {
                System.out.println("Your guess is too low");
            } else if (x == random1) {
                System.out.println("Yes, the number is " + random1);
            }
        } while (x != random1);
    }
}
