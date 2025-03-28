# Estruturas condicionais

Comandos condicionais são estruturas fundamentais em qualquer linguagem de programação, pois permitem que o programa **tome decisões** com base em condições lógicas. Em Dart, as principais estruturas condicionais são: `if`, `else if`, `else` e o **operador condicional ternário**.

## :green\_book: Estrutura `if`

A estrutura `if` permite que um bloco de código seja executado **somente se** uma condição for verdadeira.

### Sintaxe

```dart
if (condição) {
  // bloco de código
}
```

### Exemplo

```dart
int idade = 18;

if (idade >= 18) {
  print("Maior de idade");
}
```

## Estrutura `if` ... `else`

O bloco `else` é executado **caso a condição do `if` seja falsa**.

### Sintaxe

```dart
if (condição) {
  // se a condição for verdadeira
} else {
  // se a condição for falsa
}
```

```dart
bool aprovado = false;

if (aprovado) {
  print("Parabéns, você foi aprovado!");
} else {
  print("Você não foi aprovado.");
}
```

## :green\_book: Estrutura `if` ... `else if` ... `else`

Utiliza-se o `else if` para **avaliar múltiplas condições de forma encadeada**. O primeiro bloco cuja condição for verdadeira será executado; os demais serão ignorados.

### Sintaxe

```dart
if (condição1) {
  // bloco 1
} else if (condição2) {
  // bloco 2
} else {
  // bloco padrão
}
```

### Exemplo

```dart
int nota = 75;

if (nota >= 90) {
  print("Excelente");
} else if (nota >= 70) {
  print("Bom");
} else if (nota >= 50) {
  print("Regular");
} else {
  print("Reprovado");
}
```

## :green\_book: Operador Condicional Ternário

Permite escrever expressões condicionais de forma **concisa**, em uma única linha.

### Sintaxe

```dart
condição ? valor_se_verdadeiro : valor_se_falso;
```

### Exemplo

```dart
int idade = 20;
String status = (idade >= 18) ? "Adulto" : "Menor de idade";
print(status);
```

{% hint style="warning" %}
## Importante

Este operador é útil para expressões simples, mas deve ser evitado em decisões complexas.
{% endhint %}

## :green\_book: Boas Práticas

* Garantir que as condições testadas retornem **valores booleanos** (`true` ou `false`);
* Evitar duplicação de código em múltiplos blocos `if`;
* Preferir estruturas mais simples e legíveis;
* Utilizar parênteses, mesmo que não obrigatórios, para deixar a lógica mais clara.

## :pencil2: Exercícios&#x20;

1. Escreva um programa que leia a idade de uma pessoa e diga se ela é **menor de idade**, **adulta** ou **idosa** (60+ anos).
2. Crie um algoritmo que receba duas notas e calcule a média. Em seguida, informe se o aluno está **aprovado**, **em recuperação** ou **reprovado**.
3. Utilize o operador ternário para imprimir "Par" ou "Ímpar" com base em um número fornecido.
