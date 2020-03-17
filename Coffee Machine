package machine;

import java.util.Scanner;
import java.lang.Math;
public class CoffeeMachine {
    
    public static void printAmount(int water, int milk, int coffee, int cups, int money){
         System.out.println("The coffee machine has:");
         System.out.println(water+" of water");
         System.out.println(milk+" of milk");
         System.out.println(coffee+" of coffee beans");
         System.out.println(cups+" of disposable cups");
         System.out.println(money+" of money");
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Write action (buy, fill, take, remaining, exit): ");
        String action=sc.next();
        int water=400;
        int milk=540;
        int coffee=120;
        int cups=9;
        int money=550;
        
        
       
        while(!action.equals("exit"))
        {
            
            switch(action)
            {
                case "buy":
                    System.out.println("What do you want to buy? 1 - espresso, 2 - latte, 3 - cappuccino, back - to main menu: ");
                    String a=sc.next();
                    switch(a)
                    {
                        case "1":
                            if(water>=250 && coffee>=16)
                            {
                                System.out.println("I have enough resources, making you a coffee!");
                                money+=4;
                                water-=250;
                                coffee-=16;
                                cups--;
                            }
                            else
                            {
                                System.out.println("Sorry, not enough water!");
                            }
                            break;
                        case "2":
                            if(water>=350 && milk>=75 && coffee>=20)
                            {
                                System.out.println("I have enough resources, making you a coffee!");
                                money+=7;
                                water-=350;
                                milk-=75;
                                coffee-=20;
                                cups--;
                            }
                            else
                            {
                                System.out.println("Sorry, not enough water!");
                            }
                            break;
                        case "3":
                            if(water>=200 && milk>=100 && coffee>=12)
                            {
                                System.out.println("I have enough resources, making you a coffee!");
                                money+=6;
                                water-=200;
                                milk-=100;
                                coffee-=12;
                                cups--;
                            }
                            else
                            {
                                System.out.println("Sorry, not enough water!");
                            }
                            break;
                        case "back":
                            break;
                    }
                    break;
                case "fill":
                    System.out.println("Write how many ml of water do you want to add: ");
                    int l=sc.nextInt();
                    water+=l;
                    System.out.println("Write how many ml of milk do you want to add: ");
                    int m=sc.nextInt();
                    milk+=m;
                    System.out.println("Write how many grams of coffee beans do you want to add: ");
                    int n=sc.nextInt();
                    coffee+=n;
                    System.out.println("Write how many disposable cups of coffee do you want to add: ");
                    int o=sc.nextInt();
                    cups+=o;
                    break;
                case "take":
                    System.out.println("I gave you $"+money);
                    money=0;
                    break;
                case "remaining": 
                    printAmount(water,milk,coffee,cups,money);
                    break;
                case "exit":
                    break;
            }
            System.out.println("Write action (buy, fill, take, remaining, exit): ");
            action=sc.next(); 
        }
         
        
        
        
         
         
         
        
    }
}
