# Hackathone1-java
# Hackathone1-java
import java.util.Scanner;

class RooftopSolar {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int panelId = 101;
        double energyGenerated = 12.5;
        int numberOfPanels = 20;
        char systemStatus = 'A';

        System.out.println("Panel ID: " + panelId);
        System.out.println("Energy Generated: " + energyGenerated + " kWh");
        System.out.println("Number of Solar Panels: " + numberOfPanels);
        System.out.println("System Status: " + systemStatus);
    }
}

class EnergyMonitor {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter energy generated in kWh: ");
        double energy = sc.nextDouble();

        if (energy >= 10) {
            System.out.println("Good Energy Generation");
        } else {
            System.out.println("Low Energy Generation");
        }
    }
}
class SolarEnergy {
    
    static double calculateTotalEnergy(double morningEnergy, double eveningEnergy) {
        return morningEnergy + eveningEnergy;
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter morning energy: ");
        double morningEnergy = sc.nextDouble();

        System.out.print("Enter evening energy: ");
        double eveningEnergy = sc.nextDouble();

        double total = calculateTotalEnergy(morningEnergy, eveningEnergy);

        System.out.println("Total Energy Generated: " + total + " kWh");
    }
}
