# Estruturas de repetição

Os comandos de repetição permitem que blocos de código sejam executados **múltiplas vezes**, com base em uma condição lógica ou uma estrutura de controle.&#x20;

## :green\_book: Estrutura `for`

O laço `for` é utilizado quando se **conhece previamente** o número de iterações. Sua sintaxe é composta por três partes: inicialização, condição de parada e incremento.

### Sintaxe

```dart
for (inicialização; condição; incremento) {
  // bloco de código repetido
}
```

### Exemplo

```dart
for (int i = 1; i <= 5; i++) {
  print("Valor de i: $i");
}
```

## :green\_book: Estrutura `while`

O `while` é usado quando **não se sabe ao certo** quantas vezes o bloco deve ser repetido. Ele avalia a condição **antes** de cada execução.

### Sintaxe

```dart
while (condição) {
  // bloco de código repetido
}
```

### Exemplo

```dart
int contador = 1;

while (contador <= 5) {
  print("Contador: $contador");
  contador++;
}
```

## :green\_book: Estrutura `do-while`

Semelhante ao `while`, mas a diferença é que o `do-while` **executa o bloco pelo menos uma vez**, pois a condição é testada **após** a execução.

### Sintaxe

```dart
do {
  // bloco de código
} while (condição);
```

### Exemplo

```dart
int numero = 1;

do {
  print("Número: $numero");
  numero++;
} while (numero <= 3);
```

## :green\_book: Estrutura `for-in`

Utilizada para **percorrer coleções**, como listas (`List`), conjuntos (`Set`) ou mapas (`Map`). É a forma mais clara e direta de iterar sobre os elementos de uma coleção.

### Sintaxe

```dart
for (var elemento in colecao) {
  // bloco de código
}
```

### Exemplo

```dart
List<String> frutas = ["Maçã", "Banana", "Laranja"];

for (var fruta in frutas) {
  print("Fruta: $fruta");
}
```

## :green\_book: Estruturas de controle

### :small\_orange\_diamond: Comando `break`

Encerra o laço imediatamente, independentemente da condição.

```dart
for (int i = 0; i < 10; i++) {
  if (i == 5) break;
  print(i);
}
// Saída: 0 1 2 3 4
```

### :small\_orange\_diamond: Comando `continue`

Interrompe a iteração atual e passa para a **próxima repetição**.

```dart
for (int i = 0; i < 5; i++) {
  if (i == 2) continue;
  print(i);
}
// Saída: 0 1 3 4
```

## :pencil2: Exercícios

1. Imprimir os números de 1 a 10 com `for`, `while` e `do-while`.
2. Calcular a soma dos números pares entre 1 e 50.
3. Ler números do usuário até que ele digite `0` (usar `do-while`).
4. Percorrer uma lista de nomes e imprimir apenas os que começam com a letra "A" (usar `for-in` e `continue`).
