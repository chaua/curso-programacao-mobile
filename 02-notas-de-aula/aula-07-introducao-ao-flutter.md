---
description: Conceitos iniciais sobre Flutter, história, vantagens e arquitetura.
---

# 🦋 Aula 07 - Introdução ao Flutter

{% hint style="info" %}
## Material da aula

* [Slides](slides/Aula07%20-%20Introdu%C3%A7%C3%A3o%20ao%20Flutter.pdf)
{% endhint %}

## **Introdução**

O Flutter é um framework open-source criado pela Google, projetado para o desenvolvimento de interfaces gráficas modernas e responsivas com uma única base de código para múltiplas plataformas. Essa tecnologia vem ganhando destaque no desenvolvimento mobile por permitir aplicações com desempenho próximo ao nativo, reduzindo o tempo de desenvolvimento e os custos com manutenção. Esta aula apresenta os fundamentos do Flutter, sua arquitetura, funcionamento e vantagens.

## **1. O que é Flutter?**

* Framework da Google para desenvolvimento **multiplataforma**.
* Permite criar aplicativos para **Android, iOS, Web e Desktop**.
* Utiliza a linguagem **Dart**.
* Foco na produtividade do desenvolvedor e consistência visual.

## **2. Histórico e Motivação**

* Primeira versão estável lançada em **2018**.
* Criado para **resolver a fragmentação entre plataformas**.
* Alternativa aos frameworks híbridos, com **maior desempenho e controle visual**.

## **3. Benefícios para o Desenvolvedor**

* **Hot Reload**: permite alterações em tempo real sem reiniciar o app.
* **Consistência visual** entre diferentes plataformas.
* Uso de **widgets personalizáveis** e reaproveitáveis.
* Ampla comunidade e suporte corporativo (Google, Nubank, Alibaba).

## **4. Arquitetura do Flutter**

Composta por **três camadas principais**:

* **Framework (Dart)**: lógica da aplicação, UI, navegação, animações.
* **Engine (C++)**: renderização com Skia, animações, integração com Dart.
* **Embedder (nativo)**: integração com SO (entrada do usuário, câmera, GPS, etc.).

### Widgets

* Elementos básicos da interface: **tudo é um widget**.
* Tipos:
  * **StatelessWidget**: sem estado.
  * **StatefulWidget**: com estado interno.
* Organizados em **árvores de widgets** (Widget Tree).
* Permitem layout altamente modular e reativo.

### Motor Gráfico Skia

* Permite desenhar cada pixel diretamente na tela.
* Elimina dependência de componentes nativos.
* Garante **alto desempenho e fluidez** gráfica.

## **5. Linguagem Dart**

* Linguagem moderna, criada pela Google.
* Suporte a **compilação JIT (desenvolvimento)** e **AOT (produção)**.
* Fortemente tipada, mas com **inferência de tipos**.
* Excelente suporte a **programação assíncrona** com `async/await`.

## **6. Desenvolvimento com Flutter**

* Requisitos:
  * **Flutter SDK** instalado.
  * IDE como **VS Code** ou **Android Studio**.
  * Android SDK ou Xcode (para iOS).
* Ferramentas:
  * `flutter doctor`: diagnostica o ambiente de desenvolvimento.
  * Emuladores e dispositivos físicos para testes.

## **7. Vantagens do Flutter**

* Código único para várias plataformas.
* Hot Reload que **aumenta a produtividade**.
* UI rica e customizável.
* Desempenho próximo ao nativo.
* Suporte a múltiplos dispositivos (mobile, web, desktop).

## **8. Desvantagens do Flutter**

* **Tamanho elevado do APK inicial** (devido à engine embutida).
* Integração com código nativo pode ser complexa.
* Algumas APIs ainda têm suporte limitado.
* Suporte web/desktop em evolução.
* Curva de aprendizado da linguagem Dart.

## **Conclusão**

O Flutter consolida-se como uma das soluções mais completas para desenvolvimento multiplataforma. Oferece alta produtividade, UI avançada e desempenho robusto. Apesar de certas limitações, é uma excelente escolha para projetos que demandam velocidade, alcance e interface moderna.

## **Referências**

* Flutter – Site Oficial: [https://flutter.dev](https://flutter.dev)
* Dart Language – Site Oficial: [https://dart.dev](https://dart.dev)
* Pub.dev – Gerenciador de Pacotes: [https://pub.dev](https://pub.dev)
* Documentação Oficial: [https://docs.flutter.dev](https://docs.flutter.dev)

