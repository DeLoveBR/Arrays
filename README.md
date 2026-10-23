
public class Arrays {
    public static void main(String[] args) {

        // Declaração de variáveis do tipo double para armazenar
        // as temperaturas registradas em nove dias.
        double tempDia001 = 31.3;
        double tempDia002 = 32;
        double tempDia003 = 33.7;
        double tempDia004 = 34;
        double tempDia005 = 33.1;
        double tempDia006 = 32.8;
        double tempDia007 = 30;
        double tempDia008 = 29.8;
        double tempDia009 = 31.5;

        // Cria um array de double com 365 posições,
        // representando os dias de um ano.
        double[] temperaturas = new double[365];

        // Armazena as temperaturas nas posições do array.
        // Em Java, os índices começam em zero.
        temperaturas[0] = tempDia001; // Dia 1
        temperaturas[1] = tempDia002; // Dia 2
        temperaturas[2] = tempDia003; // Dia 3
        temperaturas[3] = tempDia004; // Dia 4
        temperaturas[4] = tempDia005; // Dia 5
        temperaturas[5] = tempDia006; // Dia 6
        temperaturas[6] = tempDia007; // Dia 7
        temperaturas[7] = tempDia008; // Dia 8
        temperaturas[8] = tempDia009; // Dia 9

        // Exibe o valor armazenado no índice 4,
        // que corresponde ao quinto dia.
        System.out.println(
                "O valor da temperatura do dia 4 é: " + temperaturas[3]
        );

        // Exibe a quantidade total de posições do array.
        System.out.println("O tamanho do array: " + temperaturas.length);

        // Percorre todas as posições do array utilizando o for-each.
        // A variável temp recebe o valor de cada posição a cada repetição.
        for (double temp : temperaturas) {
            System.out.println(temp);
        }

    }
}
