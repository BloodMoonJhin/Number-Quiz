package univention;

import java.util.Scanner;
import java.util.Random;

public class Univention {

    
    public static void main(String[] args) {
        
      Random randomNumber = new Random(); 
      int newNumber = randomNumber.nextInt(101);
      final int ourNumber = newNumber; 
      
      System.out.println("Please enter a number between 0-100");
      Scanner sc = new Scanner(System.in);
      int usersNumber = sc.nextInt();
      
      while(usersNumber != ourNumber){
          if (usersNumber < ourNumber){
              System.out.println("your number is smaller than the right number! Do not give up, Enter a new number!");
              usersNumber = sc.nextInt();
          }else{
              System.out.println("your number is bigger than the right number!! Do not give up, Enter a new number!");
              usersNumber = sc.nextInt();
         }
      } System.out.println("Congratulations you picked the right number!");
    }
      
      
      
      
