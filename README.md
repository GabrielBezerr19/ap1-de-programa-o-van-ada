import java.util.ArrayList;
import java.util.Collections;
import java.util.List;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Parte A: Captura e ordenação de seis números inteiros
        System.out.println("Parte A: Insira seis números inteiros:");
        List<Integer> inteiros = new ArrayList<>();
        for (int i = 0; i < 6; i++) {
            inteiros.add(scanner.nextInt());
        }
        Collections.sort(inteiros);
        System.out.println("Números inteiros em ordem crescente:");
        for (int num : inteiros) {
            System.out.println(num);
        }

        // Parte B: Captura e ordenação de seis números com casa decimal
        System.out.println("Parte B: Insira seis números com casa decimal:");
        List<Double> decimais = new ArrayList<>();
        for (int i = 0; i < 6; i++) {
            decimais.add(scanner.nextDouble());
        }
        Collections.sort(decimais);
        System.out.println("Números com casa decimal em ordem crescente:");
        for (double num : decimais) {
            System.out.println(num);
        }

        // Parte C: Captura e ordenação de seis nomes de pessoas
        System.out.println("Parte C: Insira seis nomes de pessoas:");
        List<String> nomes = new ArrayList<>();
        for (int i = 0; i < 6; i++) {
            nomes.add(scanner.next());
        }
        Collections.sort(nomes);
        System.out.println("Nomes em ordem alfabética:");
        for (String nome : nomes) {
            System.out.println(nome);
        }

        scanner.close();
    }
}
