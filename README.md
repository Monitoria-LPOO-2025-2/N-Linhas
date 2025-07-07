# Atividade N-Linhas

## Descrição da Atividade

Esta é uma atividade de autograding para implementar um gerador de padrões em Java. Sua tarefa é completar a implementação do método `gerar(int n)` na classe `GeradorLinhas` para que ele produza um padrão numérico específico.

### O Padrão Numérico

O padrão é definido da seguinte forma: para um `n`, são geradas `n` linhas. A linha `i` contém o número `i` repetido `i` vezes.

- Para n = 4, a saída deve ser:

1
22
333
4444

### Requisitos

Sua implementação deve:

1.  **Gerar o padrão correto** para os casos de teste, incluindo `n=0`, `n=1`, `n=4` e `n=5`.
2.  **Lidar com casos de borda**:
    - Funcionar corretamente para o caso base `n=0` (retornando uma string vazia).
    - Lidar com números negativos, tratando-os como se fossem `n=0` (retornando uma string vazia).
3.  **Seguir a estrutura de código existente**:
    - Implementar o método de instância `gerar(int n)` na classe `GeradorLinhas`.
    - Não modificar os arquivos de teste ou o construtor.
    - A classe `Main` pode ser usada para demonstrar sua implementação.

### Requisitos do Sistema

- Java 8 ou superior
- Gradle (wrapper incluído)

### Dependências

- JUnit Jupiter (para testes)

### Estrutura do Projeto

```text
src/
├── main/java/solution/
│   ├── GeradorLinhas.java      # Sua implementação vai aqui
│   └── Main.java               # Usado para testes manuais
└── test/java/solution/
    └── TestGeradorLinhas.java  # Casos de teste (não modificar)

