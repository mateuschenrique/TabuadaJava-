[22:34, 25/04/2024] mateus zoli: }
[22:54, 25/04/2024] mateus zoli: package tabuada.java;
import java.util.Scanner;

/**
 *
 * @author MPC
 */
public class TabuadaJava {

    private static Scanner scanner;

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
             int numero;
        try (Scanner scanner = new Scanner(System.in) // Criando um objeto Scanner
                ) {
            System.out.println("Digite um número para ver a tabuada: ");
            numero = scanner.nextInt(); // Lendo um número digitado pelo usuário
            // Fechando o Scanner após o uso
        }
        
        for (int i = 1; i <= 10; i++) {
            int resultado = numero * i;
            System.out.println(numero + " x " + i + " = " + resultado); 
        }
        }
    }
}
