# Tipos de Dados

A linguagem Dart é **fortemente tipada**, o que significa que cada valor em tempo de execução possui um tipo bem definido. Isso permite maior controle sobre o comportamento das variáveis, auxilia na detecção precoce de erros e melhora a legibilidade do código.

Dart também possui **inferência de tipos**, o que significa que o compilador pode deduzir o tipo de uma variável com base no valor atribuído, mesmo que o tipo não seja especificado de forma explícita.

## :green\_book: Tipos de Dados Primitivos

Abaixo estão os principais tipos de dados primitivos em Dart, acompanhados de exemplos e explicações.

### :1234: Números inteiros

Armazena valores inteiros positivos ou negativos, sem parte decimal.

```dart
int idade = 30;
int temperatura = -5
```

### :1234: Números de ponto flutuante

Representa valores numéricos com casas decimais (ponto flutuante).

```dart
double altura = 1.75;
double preco = 99.90;
```

> Em Dart, todos os valores decimais são do tipo `double`, não existe o tipo `float` como em outras linguagens.

### :1234: Cadeia de caracteres

Representa uma sequência de caracteres (texto).

```dart
String nome = "Maria";
String curso = 'Análise e Desenvolvimento de Sistemas';
```

> As strings podem ser delimitadas por aspas simples ou duplas.

Dart também permite **interpolação de strings**:

```dart
String saudacao = "Olá";
String nome = "Carlos";
print("$saudacao, $nome!");
```

### :1234: Valores booleanos

Representa valores lógicos: `true` (verdadeiro) ou `false` (falso).

```dart
bool ativo = true;
bool aprovado = false;
```
