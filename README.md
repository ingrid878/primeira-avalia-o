import java.util.Scanner;

public class ConversorTemperatura {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Entrada do usuário
        System.out.print("Digite a temperatura em Celsius (°C): ");
        double celsius = sc.nextDouble();

        // Conversões
        double fahrenheit = (celsius * 9/5) + 32;
        double kelvin = celsius + 273.15;

        // Saída formatada
        System.out.println("\n===== RESULTADO DA CONVERSÃO =====");
        System.out.println("Temperatura em Celsius: " + celsius + " °C");
        System.out.println("Temperatura em Fahrenheit: " + String.format("%.2f", fahrenheit) + " °F");
        System.out.println("Temperatura em Kelvin: " + String.format("%.2f", kelvin) + " K");

        sc.close();
    }
}
