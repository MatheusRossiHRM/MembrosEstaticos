# MembrosEstaticos - JAVA

package Front;

import Back.Calculator;

import java.util.Scanner;

public class Interface {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("What is the dollar price? ");
        double price = sc.nextDouble();

        System.out.println("How many dollars will be bought? ");
        double quantity = sc.nextDouble();

        System.out.printf("Amount to be paid in reais = %.2f%n", Calculator.soma(price, quantity));

        sc.close();
    }
}


package Back;

public class Calculator {

    public static final double soma (double price, double quantity){
        return price * quantity * 0.06 + price * quantity;
    }

}

