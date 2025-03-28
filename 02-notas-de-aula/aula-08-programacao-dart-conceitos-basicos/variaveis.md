# Variáveis

Em programação, uma **variável** é um espaço reservado na memória que armazena um valor que pode ser lido, modificado ou utilizado ao longo da execução do programa. Na linguagem Dart, a declaração de variáveis segue uma sintaxe clara, podendo ser **explícita** (com definição do tipo) ou **implícita** (com inferência de tipo).

## :green\_book: Declaração Explícita

Na declaração explícita, o tipo da variável é informado antes do identificador (nome da variável).

```dart
int idade = 25;
double altura = 1.75;
String nome = "Carlos";
bool matriculado = true;
```

Cada linha acima segue a estrutura:

```
<tipo> <nome_da_variável> = <valor>;
```

{% hint style="success" %}
## Dica

Este tipo de declaração é útil para reforçar a clareza e a tipagem do código, além de facilitar a manutenção em projetos maiores.
{% endhint %}

## :green\_book: Inferência de Tipo com `var`

Ao utilizar a palavra-chave `var`, o compilador de Dart infere automaticamente o tipo da variável com base no valor atribuído no momento da declaração.

```dart
var curso = "Ciência da Computação"; // Inferido como String
var nota = 8.5;                      // Inferido como double
```

{% hint style="warning" %}
## Importante!

Após a inferência, o tipo torna-se fixo — ou seja, a variável **não poderá assumir outro tipo de valor posteriormente**.
{% endhint %}

```dart
var idade = 20;
idade = "vinte"; // ❌ Erro: tipo incompatível
```

## :green\_book: Imutabilidade com `final` e `const`

Dart permite a criação de variáveis **imutáveis**, ou seja, cujo valor **não pode ser modificado** após a atribuição.

**🔸 `final`**

O valor é atribuído **em tempo de execução**, mas **não pode ser alterado depois**.

```dart
final String cpf = "123.456.789-00";
final agora = DateTime.now();
```

**🔸 `const`**

Atribuição de **constantes literais**, cujo valor deve ser conhecido **em tempo de compilação**.

```dart
const double pi = 3.14159;
const saudacao = "Bem-vindo!";
```

{% hint style="warning" %}
## Importante!

Diferença: `final` pode depender de chamadas dinâmicas (como data atual), enquanto `const` exige um valor literal e fixo.
{% endhint %}

## :green\_book: Declaração com `dynamic`

O tipo `dynamic` permite a criação de variáveis que podem **assumir diferentes tipos de valor** durante a execução do programa.

```dart
dynamic valor = 10;
valor = "dez";       // Permitido
valor = true;        // Também permitido
```

{% hint style="warning" %}
## Importante!

Embora `dynamic` forneça flexibilidade, seu uso indiscriminado pode comprometer a segurança do código, dificultar a depuração e causar erros em tempo de execução.
{% endhint %}

## :green\_book: Boas Práticas

* Utilizar **declaração explícita** para variáveis de escopo global ou de maior importância semântica.
* Preferir `var` quando o tipo for óbvio, para evitar redundância.
* Usar `final` e `const` sempre que o valor **não precisar ser alterado**, favorecendo a imutabilidade.
* **Evitar `dynamic`**, salvo quando a flexibilidade for estritamente necessária.
