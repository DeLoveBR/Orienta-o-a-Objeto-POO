
// Importa a classe ArrayList para armazenar as tarefas
import java.util.ArrayList;

// Importa a classe Scanner para receber dados digitados pelo usuário
import java.util.Scanner;

public class Main {

    public static void main(String[] args) throws Exception {

        // Cria um Scanner para ler as informações digitadas no teclado
        Scanner scanner = new Scanner(System.in);

        // Cria uma lista dinâmica para armazenar as tarefas
        ArrayList<String> tarefas = new ArrayList<>();

        // Variável responsável por armazenar a opção escolhida pelo usuário
        int opcao;

        // O do-while mantém o menu funcionando até o usuário escolher sair
        do {

            // Exibe o menu principal do programa
            System.out.println("\n=== GERENCIADOR DE TAREFAS ===");
            System.out.println("1. Adicionar tarefa");
            System.out.println("2. Listar tarefas");
            System.out.println("3. Excluir tarefa");
            System.out.println("0. Sair");
            System.out.print("Escolha uma opção: ");

            // Lê a opção escolhida pelo usuário
            opcao = scanner.nextInt();

            // Limpa a quebra de linha que fica no buffer do Scanner
            scanner.nextLine();

            // O switch verifica qual opção foi escolhida
            switch (opcao) {

                // Opção 1: Adicionar uma nova tarefa
                case 1:

                    // Solicita ao usuário o nome da tarefa
                    System.out.print("Digite a tarefa: ");

                    // Armazena o texto digitado em uma variável
                    String tarefa = scanner.nextLine();

                    // Adiciona a tarefa na lista
                    tarefas.add(tarefa);

                    System.out.println("Tarefa adicionada com sucesso!");
                    break;

                // Opção 2: Listar todas as tarefas cadastradas
                case 2:

                    System.out.println("\n=== LISTA DE TAREFAS ===");

                    // Percorre a lista utilizando um laço for
                    for (int i = 0; i < tarefas.size(); i++) {

                        // Exibe o número e a descrição de cada tarefa
                        System.out.println((i + 1) + ". " + tarefas.get(i));
                    }
                    break;

                // Opção 3: Excluir uma tarefa
                case 3:

                    // Solicita o número da tarefa que será excluída
                    System.out.print("Digite o número da tarefa a ser excluída: ");

                    // Subtrai 1 porque as posições da lista começam em zero
                    int indice = scanner.nextInt() - 1;

                    // Verifica se o índice informado existe na lista
                    if (indice >= 0 && indice < tarefas.size()) {

                        // Remove a tarefa da posição informada
                        tarefas.remove(indice);

                        System.out.println("Tarefa excluída com sucesso!");

                    } else {

                        // Informa ao usuário quando o número é inválido
                        System.out.println("Número inválido!");
                    }
                    break;

                // Opção 0: Encerrar o programa
                case 0:

                    System.out.println("Saindo do programa...");
                    break;

                // Executado quando o usuário digita uma opção inexistente
                default:

                    System.out.println("Opção inválida! Tente novamente.");
            }

        // Repete o menu enquanto a opção escolhida for diferente de zero
        } while (opcao != 0);

        // Fecha o Scanner ao finalizar o programa
        scanner.close();
    }
}
