# Health Assistant
import java.util.Scanner;

public class HealthAssistant {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Health Program!");
        System.out.print("Please enter your age: ");
        int age = scanner.nextInt();

        if (age < 65) {
            System.out.println("This program is designed for individuals aged 65 or above. Exiting the program.");
            System.exit(0);
        }

        while (true) {
            System.out.println("\nPlease select an area of focus:");
            System.out.println("1. Exercise");
            System.out.println("2. Nutrition");
            System.out.println("3. Mental Well-being");
            System.out.println("4. Preventive Measures");
            System.out.println("5.Regular Check-up's");
            System.out.println("0. Exit");

            System.out.print("Enter your choice: ");
            int choice = scanner.nextInt();

            switch (choice) {
                case 1:
                    displayExerciseRecommendations();
                    break;
                case 2:
                    displayNutritionRecommendations();
                    break;
                case 3:
                    displayMentalWellBeingRecommendations();
                    break;
                case 4:
                    displayPreventiveMeasureRecommendations();
                    break;
                case 5:
                    displayRegulationCheckups();
                    break;
                case 0:
                    System.out.println("Exiting the program.");
                    System.exit(0);
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }

    public static void displayExerciseRecommendations() {
        System.out.println("\nExercise Recommendations:");
        System.out.println("- Walk for 30 minutes daily.");
        System.out.println("- Engage in light strength training exercises.");
        System.out.println("- Try yoga or stretching exercises.");
    }

    public static void displayNutritionRecommendations() {
        System.out.println("\nNutrition Recommendations:");
        System.out.println("- Consume a balanced diet with plenty of fruits and vegetables.");
        System.out.println("- Opt for whole grains and limit processed foods.");
        System.out.println("- Control portion sizes and avoid excess sugar and salt.");
    }

    public static void displayMentalWellBeingRecommendations() {
        System.out.println("\nMental Well-being Recommendations:");
        System.out.println("- Practice meditation or deep breathing exercises.");
        System.out.println("- Engage in activities you enjoy, such as reading or hobbies.");
        System.out.println("- Spend quality time with loved ones and maintain a strong support network.");
    }

    public static void displayPreventiveMeasureRecommendations() {
        System.out.println("\nPreventive Measures Recommendations:");
        System.out.println("- Schedule regular health check-ups and screenings.");
        System.out.println("- Stay up-to-date with vaccinations.");
        System.out.println("- Follow medical advice and take necessary preventive measures.");
    }
    public static void displayRegulationCheckups(){
        System.out.println("\nRegular Health check-up:");
        System.out.println("- Schedule regular Health check-ups with your healthcare provider.");
        System.out.println("- Monitoring your blood pressure, cholesterol levels and other vital health indicators for early detection and and better management of any potential health issues.");
    }
}

