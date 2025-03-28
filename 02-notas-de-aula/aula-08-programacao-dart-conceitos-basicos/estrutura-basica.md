# Estrutura básica

Dart segue uma sintaxe simples e expressiva, herdada de linguagens como JavaScript, Java e C#. O ponto de partida de qualquer programa Dart é a função principal, denominada `main()`.

## :green\_book: Alô, mamãe!

```dart
void main() {
  print('Alô, mamãe!');
}
```

### Explicação da estrutura

| Componente      | Descrição                                                                             |
| --------------- | ------------------------------------------------------------------------------------- |
| `void`          | Palavra-chave que indica que a função `main()` **não retorna nenhum valor**.          |
| `main()`        | Função principal. É o **ponto de entrada obrigatório** de qualquer programa Dart.     |
| `{ ... }`       | Bloco de código delimitado por chaves, contendo as instruções que serão executadas.   |
| `print(...)`    | Função utilizada para **exibir mensagens no console**. Ideal para testes e depuração. |
| `'Olá, mundo!'` | String literal, delimitada por aspas simples ou duplas.                               |

***

## :green\_book: Ambiente de desenvolvimento

Para fins de aprendizado e testes iniciais, recomenda-se fortemente o uso do ambiente online chamado **DartPad**, uma ferramenta oficial da Google.

{% hint style="info" %}
## DartPad

* &#x20;[https://dartpad.dev](https://dartpad.dev)
{% endhint %}

### Como utilizar o DartPad

1. Acessar o site [https://dartpad.dev](https://dartpad.dev);
2. Substituir o código de exemplo pelo seu próprio;
3. Pressionar o botão **"Run"** (ou **Executar**) para ver o resultado no console à direita.
