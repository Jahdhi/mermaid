package shdlproject;

import java.util.Scanner;
import java.util.InputMismatchException;

public class Airline {

    public int airlineNumber;

    public void displayAirline() {
        System.out.println("""
                           1.Saudi Arabian Airlines
                           2.Flynas
                           3.SaudiGulf Airlines
                           4.Flyadeal
                           """);
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter your choice :");
            airlineNumber = scanner.nextInt();
            int n = airlineNumber;
            switch (n) {
                case 1:
                    System.out.println("\nWelcome to Saudi Arabian Airlines!\n");
                    break;
                case 2:
                    System.out.println("\nWelcome to Flynas!\n");
                    break;
                case 3:
                    System.out.println("\nWelcome to SaudiGulf Airlines!\n");
                    break;
                case 4:
                    System.out.println("\nWelcome to Flyadeal!\n");
                    break;

                default:

                    System.out.println("The number you entered is out of range.\n");
                    System.out.println("Please enter 1-4 to choose your airline flight\n");
                    displayAirline();

            }
        }

    

    public void ContactINF() {
        System.out.println("Contact us at:");
        switch (airlineNumber) {
            case 1:
                System.out.println("Saudi Arabian Airline\\nswww.saudiairlines.com\n" + "Phone: 123-456-7890");
                break;
            case 2:
                System.out.println("Flynaswww.flynas.com\n" + "Phone: 123-456-7890");
                break;
            case 3:
                System.out.println("SaudiGulf Airlineswww.saudigulfairlines.com\n" + "Phone: 123-456-7890");
                break;
            case 4:
                System.out.println("Flyadealwww.flyadeal.com\n" + "Phone: 123-456-7890");
                break;
            default:
                System.out.println("SaudiGulf Airlineswww.saudigulfairlines.com\n" + "Phone: 123-456-7890");
        }
    }
}
