# 🌡️ Manipulação de Arrays com Temperaturas em Java

Este projeto consiste em um programa em Java focado no aprendizado e manipulação de **estruturas de dados estáticas (Arrays)**. O algoritmo simula o armazenamento e a leitura de temperaturas registradas ao longo dos dias de um ano.

## 📋 Cenário do Problema

O objetivo do programa é praticar os conceitos fundamentais de vetores em Java:
* **Alocação de Memória:** Criação de um array de ponto flutuante (`double[]`) com capacidade fixa para **365 posições** (representando os dias do ano).
* **Indexação:** Atribuição manual de temperaturas nas primeiras posições do vetor, respeitando a regra de que os índices em Java começam em **0**.
* **Leitura de Dados:** Acesso direto a um índice específico e verificação do tamanho total do array via atributo `.length`.
* **Iteração:** Uso do laço de repetição **for-each** para percorrer e exibir os dados armazenados de forma limpa.

---

## 💻 Código Fonte

Abaixo está o código organizado dentro de uma classe executável. Foi adicionado um filtro no laço `for-each` para imprimir apenas os dias que possuem temperaturas registradas (diferentes de zero).

```java
public class RegistroTemperaturas {
    public static void main(String[] args) {
        // Declaração de variáveis para armazenar as temperaturas registradas
        double tempDia001 = 31.3;
        double tempDia002 = 32;
        double tempDia003 = 33.7;
        double tempDia004 = 34;
        double tempDia005 = 33.1;
        double tempDia006 = 32.8;
        double tempDia007 = 30;
        double tempDia008 = 29.8;
        double tempDia009 = 31.5;

        // Cria um array de double com 365 posições (representando os dias de um ano)
        double[] temperaturas = new double[365];

        // Armazena as temperaturas nas primeiras posições do array (índices começam em 0)
        temperaturas[0] = tempDia001; // Dia 1
        temperaturas[1] = tempDia002; // Dia 2
        temperaturas[2] = tempDia003; // Dia 3
        temperaturas[3] = tempDia004; // Dia 4
        temperaturas[4] = tempDia005; // Dia 5
        temperaturas[5] = tempDia006; // Dia 6
        temperaturas[6] = tempDia007; // Dia 7
        temperaturas[7] = tempDia008; // Dia 8
        temperaturas[8] = tempDia009; // Dia 9

        // Exibe o valor armazenado no índice 3, que corresponde ao quarto dia
        System.out.println("O valor da temperatura do dia 4 é: " + temperaturas[3] + "°C");

        // Exibe a quantidade total de posições alocadas no array
        System.out.println("O tamanho total do array: " + temperaturas.length + " posições");

        System.out.println("\n--- Temperaturas Registradas ---");
        // Percorre o array utilizando o for-each.
        for (double temp : temperaturas) {
            // Filtro para exibir apenas posições preenchidas (Java inicializa double[] com 0.0)
            if (temp != 0.0) {
                System.out.println(temp + "°C");
            }
        }
    }
}
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Você precisará do [JDK (Java Development Kit)](https://oracle.com) instalado na sua máquina (versão 8 ou superior).

### Passo a Passo

1. **Crie o arquivo:** Salve o código acima em um arquivo chamado `RegistroTemperaturas.java`.
2. **Abra o terminal:** Navegue até a pasta onde o arquivo foi salvo.
3. **Compile o código:**
   ```bash
   javac RegistroTemperaturas.java
   ```
4. **Execute o programa:**
   ```bash
   java RegistroTemperaturas
   ```

---

## 📝 Conceitos Praticados

* Declaração e inicialização de arrays unidimensionais (vetores).
* Controle de índices baseado em zero (`0` a `length - 1`).
* Descobrimento dinâmico do tamanho de estruturas com o atributo `.length`.
* Iteração simplificada em coleções através do laço `for-each` (também conhecido como *Enhanced for*).
* Filtros condicionais (`if`) para manipulação de saídas no console.
