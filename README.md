# Atividade N-Linhas
Descrição da Atividade
Esta é uma atividade de autograding para implementar um gerador de padrões em Java. Sua tarefa é completar a implementação do método gerar(int n) na classe GeradorLinhas para que ele produza um padrão numérico específico.

O Padrão Numérico
O padrão é definido da seguinte forma: para um n, são geradas n linhas. A linha i contém o número i repetido i vezes.

Para n = 4, a saída deve ser:

1
22
333
4444
Requisitos
Sua implementação deve:

Calcular o padrão correto para os casos de teste, incluindo n=0, n=1, n=4 e n=5.

Lidar com casos de borda:

Funcionar corretamente para o caso base n=0 (retornando uma string vazia).

Lidar com números negativos, tratando-os como se fossem n=0 (retornando uma string vazia).

Seguir a estrutura de código existente:

Implementar o método de instância gerarLinhas(int n) na NLinhas.

Não modificar os arquivos de teste ou o construtor.

A classe Main deve demonstrar sua implementação.

Requisitos do Sistema
Java 8 ou superior

Gradle (wrapper incluído)

Dependências
JUnit Jupiter (para testes)

Estrutura do Projeto
Plaintext

src/
├── main/java/solution/
│   ├── GeradorLinhas.java      # Sua implementação vai aqui
│   └── Main.java               # Demonstra o uso da sua classe
└── test/java/solution/
    └── TestGeradorLinhas.java  # Casos de teste (não modificar)
Como Executar os Testes
Para rodar os testes automatizados que corrigirão sua atividade:

Bash

gradle test
Para rodar a classe principal (após a implementação):

Bash

gradle run
Estratégia de Teste
A atividade inclui:

Testes Parametrizados cobrindo múltiplos valores, como n=0, n=1, n=2, n=4 e n=5, para garantir a correção da lógica.

Teste de Caso de Borda para garantir que entradas negativas são tratadas corretamente.

Avaliação
Sua solução será avaliada automaticamente com base em:

Correção da geração do padrão.

Passagem em todos os casos de teste.

Qualidade do código e adesão às convenções Java.

Como Começar
Clone este repositório.

Implemente o método gerar(int n) em src/main/java/solution/GeradorLinhas.java.

Rode gradle test para verificar sua implementação.

Certifique-se de que todos os testes passem antes de enviar.

Dicas de Implementação
Comece tratando o caso de n negativo.

Use laços for aninhados: um para as linhas e outro para repetir os dígitos.

Lembre-se de adicionar a quebra de linha \n após cada linha (exceto a última).

Você precisará implementar um método de instância, não um método estático.

