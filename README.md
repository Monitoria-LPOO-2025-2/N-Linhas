# Atividade N-Linhas

## Visão Geral do Projeto

Bem-vindo à atividade "N-Linhas"! Este é um pequeno projeto em Java projetado para praticar seus conhecimentos de lógica de programação, especialmente o uso de laços de repetição (loops) e manipulação de strings.

O objetivo é simples: você precisa completar um método em Java que gera um padrão numérico com base em um número inteiro `n`.

## O Desafio

O padrão que você precisa criar funciona da seguinte maneira: para um dado número `n`, seu programa deve gerar `n` linhas de texto. Cada linha `i` (de 1 a `n`) deve conter o número `i` repetido `i` vezes.

**Por exemplo, se `n = 4`, a saída esperada é:**

1
22
333
4444


## Estrutura do Projeto

O projeto já vem com alguns arquivos para te ajudar. É importante que você se familiarize com eles:

```text
src
├── main
│   ├── java
│   │   ├── solution
│   │   │   ├── NLinhas.java  <-- 🎯 É AQUI QUE VOCÊ VAI TRABALHAR!
│   │   │   └── Main.java     <-- Use este para testes manuais.
└── test
    └── java
        └── solution
            └── TestNLinhas.java <-- Testes automáticos (não modifique!).
NLinhas.java: Contém a classe NLinhas com o método gerarLinhas(int n) que você precisa implementar.

Main.java: Uma classe com um método main onde você pode escrever seu próprio código para testar a sua implementação manualmente. O código aqui não será avaliado.

TestNLinhas.java: Contém os testes automatizados que serão usados para corrigir sua atividade. Você pode (e deve!) olhar este arquivo para entender todos os casos que sua solução precisa atender.

Sua Tarefa
Sua única tarefa é implementar a lógica dentro do método gerarLinhas(int n) no arquivo NLinhas.java.

O método recebe um inteiro n e deve retornar uma String com o padrão completo. Lembre-se que cada linha no padrão final deve ser separada por um caractere de nova linha (\n).

Java

public String gerarLinhas(int n) {
    // Implemente toda a sua lógica aqui.
    // DICA: Verifique se n <= 0. Se for, retorne "".
    // DICA: Use laços (loops) para construir a string linha por linha.
    // DICA: Retorne a variável que guarda a string final.

    return ""; // Substitua isso pela sua implementação
}
Requisitos
Para que sua solução seja considerada correta, ela deve:

Gerar o padrão correto para qualquer valor de n positivo.

Lidar com o caso n = 0: Se n for 0, o método deve retornar uma string vazia ("").

Lidar com números negativos: Se n for um número negativo, o comportamento deve ser o mesmo que para n = 0, retornando uma string vazia.

Seguir a estrutura de código existente: Não altere os nomes dos métodos, classes ou a estrutura dos arquivos.

Como Testar seu Código
Teste Manual
Você pode usar o arquivo Main.java para fazer testes rápidos. Descomente o código dentro do método main para ver a saída do seu método gerarLinhas no console:

Java

public static void main(String[] args) {
    // Teste seu código aqui
    NLinhas gerador = new NLinhas();
    int numeroDeLinhas = 5;
    String resultado = gerador.gerarLinhas(numeroDeLinhas);
    System.out.println("Teste para n = " + numeroDeLinhas);
    System.out.print(resultado);
}
Teste Automatizado (Correção)
O projeto está configurado com Gradle. Para rodar os testes automatizados e verificar se sua solução está correta, execute o seguinte comando no terminal, na raiz do projeto:

Bash

./gradlew test
Se todos os testes passarem, você verá uma mensagem de "BUILD SUCCESSFUL". Caso contrário, um relatório de testes será gerado na pasta build/reports/tests/test/index.html, indicando quais casos falharam.
