# Variáveis nulas

Desde a versão 2.12, Dart introduziu o recurso chamado **null safety**, ou **segurança contra valores nulos**. Isso significa que o compilador ajuda o desenvolvedor a **evitar erros causados pelo uso de variáveis que podem conter `null`**, um problema comum em várias linguagens de programação e uma das maiores fontes de exceções em tempo de execução.

Uma **variável nula** é aquela que **não possui valor atribuído** — seu valor é `null`. Em Dart, por padrão, **nenhuma variável pode ter valor nulo, a menos que seja declarada explicitamente como tal**.

## :green\_book: Declaração de variáveis não-nulas

Ao declarar uma variável com tipo explícito, assume-se que ela **sempre terá um valor não-nulo**.

```dart
int idade = 20;      // Correto
idade = null;        // Erro de compilação
```

## :green\_book: Declaração de variáveis potencialmente nulas

Para permitir que uma variável possa receber `null`, deve-se usar o **operador de interrogação `?`** após o tipo da variável.

```dart
int? idade;          // Pode ser nula
idade = null;        // Correto
idade = 30;          // Correto
```

O tipo `int?` representa um inteiro que **pode ser nulo** (`int` ou `null`).

## :green\_book: Acesso a variáves potencialmente nulas

Quando uma variável é declarada como podendo ser nula, o Dart exige que o programador trate explicitamente a possibilidade de `null`, antes de utilizá-la. Exemplo:

```dart
int? idade = null;
print(idade + 5);  // ❌ Erro: valor pode ser nulo
```

O acesso das variáveis potencialmente nulas pode ser realizadas como segue.

### :small\_orange\_diamond: **Verificação com `if`**

```dart
if (idade != null) {
  print(idade + 5);
}
```

### :small\_orange\_diamond: **Operador de coalescência nula `??`**

Utiliza um valor padrão caso o valor seja nulo.

```dart
print((idade ?? 0) + 5);  // Se idade for nula, assume 0
```

### :small\_orange\_diamond: **Operador de acesso seguro `?.`**

Usado para acessar membros (métodos ou atributos) **somente se** o objeto não for nulo.

```dart
String? nome;
print(nome?.toUpperCase());  // Evita erro se nome for null
```

### :small\_orange\_diamond: **Operador de asserção `!`**

Garante que o valor **não é nulo**, e força o acesso. Se o valor for `null`, lança um erro.

```dart
int? idade = 25;
print(idade! + 5);  // Funciona, mas cuidado! Pode lançar erro se idade for null
```

## :green\_book: Benefícios da Null Safety

* Redução de exceções em tempo de execução (como `NullPointerException`);
* Código mais robusto e seguro;
* Incentivo a boas práticas de programação defensiva;
* Verificações automáticas de nulidade durante a compilação.

## :green\_book: Tabela Resumo

<table><thead><tr><th width="232">Sintaxe</th><th>Significado</th></tr></thead><tbody><tr><td><code>int x = 10;</code></td><td><code>x</code> é um inteiro <strong>não-nulo</strong></td></tr><tr><td><code>int? y = null;</code></td><td><code>y</code> é um inteiro que <strong>pode ser nulo</strong></td></tr><tr><td><code>y ?? valor</code></td><td>Usa <code>valor</code> caso <code>y</code> seja nulo</td></tr><tr><td><code>variavel?.metodo()</code></td><td>Executa <code>metodo()</code> apenas se a variável não for nula</td></tr><tr><td><code>variavel!</code></td><td>Asserção: garante que não é nula (<strong>com risco</strong>)</td></tr></tbody></table>

## :pencil2: Exercícios

1. Declare uma variável `String? nome` e exiba uma mensagem padrão se ela for nula.
2. Crie uma função que receba um `int?` e retorne seu valor dobrado, usando `??` para tratar nulidade.
3. Simule o cadastro de um usuário com nome e email opcionais, tratando os nulos com segurança.
