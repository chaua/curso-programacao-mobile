# Operadores

Operadores são símbolos especiais que instruem o compilador a realizar operações específicas sobre um ou mais operandos. A linguagem Dart oferece uma ampla gama de operadores organizados em diferentes categorias, conforme o tipo de operação realizada.

## :green\_book: Operadores Aritméticos

São utilizados para realizar operações matemáticas básicas com variáveis do tipo `int` ou `double`.

| Operador | Significado                   | Exemplo   | Resultado  |
| -------- | ----------------------------- | --------- | ---------- |
| `+`      | Adição                        | `5 + 3`   | `8`        |
| `-`      | Subtração                     | `10 - 4`  | `6`        |
| `*`      | Multiplicação                 | `2 * 6`   | `12`       |
| `/`      | Divisão (com ponto flutuante) | `10 / 3`  | `3.333...` |
| `~/`     | Divisão inteira               | `10 ~/ 3` | `3`        |
| `%`      | Resto da divisão (módulo)     | `10 % 3`  | `1`        |
| `-a`     | Negação (valor negativo)      | `-7`      | `-7`       |

## :green\_book: Operadores Relacionais&#x20;

Comparam dois valores e **retornam um valor booleano** (`true` ou `false`).

| Operador | Significado      | Exemplo  | Resultado |
| -------- | ---------------- | -------- | --------- |
| `==`     | Igual a          | `5 == 5` | `true`    |
| `!=`     | Diferente de     | `4 != 3` | `true`    |
| `>`      | Maior que        | `7 > 2`  | `true`    |
| `<`      | Menor que        | `2 < 3`  | `true`    |
| `>=`     | Maior ou igual a | `5 >= 5` | `true`    |
| `<=`     | Menor ou igual a | `6 <= 4` | `false`   |

## :green\_book: Operadores Lógicos

São usados para construir **expressões booleanas compostas**, muito úteis em estruturas de controle.

| Operador | Significado    | Exemplo           | Resultado |
| -------- | -------------- | ----------------- | --------- |
| `&&`     | E lógico (AND) | `true && false`   | `false`   |
| `\|\|`   | OU lógico (OR) | `true \|\| false` | `true`    |
| `!`      | Negação lógica | `!true`           | `false`   |

## :green\_book: Operadores de Atribuição

| Operador | Significado                | Exemplo                |
| -------- | -------------------------- | ---------------------- |
| `=`      | Atribuição simples         | `a = 5`                |
| `+=`     | Soma e atribuição          | `a += 2` → `a = a + 2` |
| `-=`     | Subtração e atribuição     | `a -= 1` → `a = a - 1` |
| `*=`     | Multiplicação e atribuição | `a *= 3`               |
| `/=`     | Divisão e atribuição       | `a /= 2`               |

## :green\_book: Operadores de Incremento e Decremento

| Operador | Significado           | Exemplo        |
| -------- | --------------------- | -------------- |
| `++`     | Incrementa 1 ao valor | `a++` ou `++a` |
| `--`     | Decrementa 1 do valor | `a--` ou `--a` |

{% hint style="info" %}
A diferença entre `++a` e `a++` é que o primeiro incrementa **antes** de usar o valor, enquanto o segundo incrementa **depois**.
{% endhint %}

## :green\_book: Operador Condicional Ternário

Permite escrever uma condicional simples em uma única linha:

```dart
var resultado = (idade >= 18) ? "Adulto" : "Menor";
```

## :green\_book: Operador de Coalescência Nula (`??`)

Retorna o primeiro operando **não-nulo**:

```dart
String? nome;
print(nome ?? "Anônimo");  // Saída: "Anônimo"
```
