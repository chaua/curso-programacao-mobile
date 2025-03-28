# Funções

Uma **função** (ou método) é um **bloco reutilizável de código** que executa uma tarefa específica. Funções ajudam a **organizar o código**, evitar repetição, **modularizar programas** e facilitar a manutenção e o teste.

Em Dart, **todas as instruções são executadas dentro de uma função**, sendo a função `main()` o ponto de entrada obrigatório de qualquer programa.

## :green\_book: Estrutura de uma função

```dart
tipoDeRetorno nomeDaFuncao(parâmetros) {
  // corpo da função
  return valorDeRetorno;
}
```

<table><thead><tr><th width="166.5">Componente</th><th>Descrição</th></tr></thead><tbody><tr><td><code>tipoDeRetorno</code></td><td>Indica o tipo do valor retornado pela função (<code>int</code>, <code>double</code>, <code>String</code>, <code>void</code>, etc.)</td></tr><tr><td><code>nomeDaFuncao</code></td><td>Nome que identifica a função</td></tr><tr><td><code>parâmetros</code></td><td>Lista opcional de entradas que a função recebe</td></tr><tr><td><code>return</code></td><td>Palavra-chave usada para devolver um valor ao chamador</td></tr></tbody></table>

### Exemplo 1: Função com retorno e parâmetros

```dart
int somar(int a, int b) {
  return a + b;
}
```

### Exemplo 2: Função sem retorno (`void`)

```dart
void saudacao(String nome) {
  print("Olá, $nome!");
}
```

## :green\_book: Parâmetros Opcionais

Dart permite a definição de **parâmetros opcionais**, que podem ser **nomeados** ou **posicionais**.

### :small\_orange\_diamond: Parâmetros Nomeados (com chaves `{}`)

```dart
void mostrarDados({String? nome, int? idade}) {
  print("Nome: $nome, Idade: $idade");
}

void main() {
  mostrarDados(nome: "Ana", idade: 20);
}
```

É possível atribuir **valores padrão**:

```dart
void apresentar({String nome = "Visitante"}) {
  print("Bem-vindo, $nome!");
}
```

### :small\_orange\_diamond: Parâmetros Posicionais Opcionais (com colchetes `[]`)

```dart
void exibirMensagem(String mensagem, [String? autor]) {
  print("$mensagem - ${autor ?? 'Anônimo'}");
}

void main() {
  exibirMensagem("Boa noite");
  exibirMensagem("Bom dia", "Carlos");
}
```

## :green\_book: Funções lambda

Dart permite o uso de funções **sem nome**, ideais para passagens rápidas como parâmetros.

```dart
List<int> numeros = [1, 2, 3, 4];

numeros.forEach((num) {
  print("Valor: $num");
});
```

## :green\_book: Funções como Objetos de Primeira Classe

Em Dart, funções são **cidadãs de primeira classe**, ou seja:

* Podem ser atribuídas a variáveis;
* Podem ser passadas como parâmetros;
* Podem ser retornadas por outras funções.

```dart
int dobrar(int x) => x * 2;

void aplicar(Funcao f, int valor) {
  print(f(valor));
}

typedef Funcao = int Function(int);

void main() {
  aplicar(dobrar, 5); // imprime 10
}
```

## :pencil2: Exercícios&#x20;

1. Escreva uma função que receba dois números e retorne a média entre eles.
2. Implemente uma função que receba um nome e retorne uma saudação personalizada.
3. Crie uma função que verifique se um número é primo.
4. Faça uma função que receba uma lista de notas e retorne a média e a situação (Aprovado, Reprovado).
5. Implemente uma função com parâmetros opcionais que personalize uma mensagem de boas-vindas.
