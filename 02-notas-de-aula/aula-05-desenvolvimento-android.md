---
description: Introdução ao desenvolvimento de aplicativos Android.
---

# 🤖 Aula 05 - Desenvolvimento Android

{% hint style="info" %}
## Material da aula

* [Slides](slides/Aula05%20-%20Desenvolvimento%20Android.pdf)
{% endhint %}

## **Introdução**

O Android é o sistema operacional móvel mais utilizado no mundo, presente em bilhões de dispositivos. Baseado no kernel Linux e com código aberto, ele permite o desenvolvimento de aplicações para uma ampla gama de dispositivos, como smartphones, tablets, TVs e smartwatches. Esta aula apresenta uma introdução ao Android, abordando sua história, arquitetura, ferramentas de desenvolvimento, estrutura de projeto e os principais conceitos necessários para começar a programar para a plataforma.

## **1. O que é Android?**

* Sistema operacional baseado no Linux.
* Projetado para dispositivos com tela sensível ao toque.
* É um projeto de código aberto (Android Open Source Project - AOSP).
* Licenciado sob a Apache License.

## **2. Histórico e Evolução**

* Criado em 2003 pela Android Inc., adquirida pelo Google em 2005.
* Primeira versão lançada em 2007.
* Participação da **Open Handset Alliance** para padronizar o Android.
* Destaque para versões como Cupcake, Nougat, Pie, até o Android 10, com melhorias progressivas em desempenho, segurança e interface.

## **3. Fundamentos de Aplicativos Android**

* Aplicações podem ser escritas em Kotlin, Java ou C++.
* Compiladas em arquivos APK através do Android SDK.
* Cada aplicativo funciona em sua própria sandbox, garantindo segurança.
* Princípio do privilégio mínimo: acesso apenas ao necessário.
* Componentes principais:
  * **Activities**
  * **Services**
  * **Broadcast Receivers**
  * **Content Providers**

## **4. Arquitetura da Plataforma Android**

A arquitetura Android é composta por várias camadas:

* **Kernel do Linux**: gerenciamento de memória, segurança, drivers.
* **HAL (Hardware Abstraction Layer)**: interface entre software e hardware.
* **Android Runtime (ART)**: substitui o Dalvik, com AOT e JIT.
* **Bibliotecas nativas (C/C++)**: OpenGL, media framework.
* **APIs Java**: gerenciamento de UI, notificações, atividades.
* **Aplicativos do sistema**: e-mail, mensagens, calendário, etc.

## **5. Ambiente de Desenvolvimento**

* **Android Studio**: IDE oficial, baseada no IntelliJ IDEA.
  * Suporte a todas as ferramentas necessárias.
  * Compilação com Gradle.
  * Testes, debug e publicação integrados.
* **JDK**: necessário para desenvolvimento Java/Kotlin.
* Ferramentas auxiliares:
  * **SDK Manager**: gerencia versões do Android.
  * **AVD Manager**: cria emuladores de dispositivos.

## **6. Estrutura de um Projeto Android**

Um projeto Android é composto por:

* **AndroidManifest.xml**: define permissões, componentes e requisitos.
* **Código-fonte**: Java ou Kotlin, organizados por pacotes.
* **Recursos estáticos**: organizados em diretórios como:
  * `/layout`: layouts das telas.
  * `/drawable`: imagens.
  * `/values`: textos, cores, dimensões, estilos.
  * `/mipmap`: ícones.
* **Qualificadores**: recursos adaptados para diferentes configurações (idioma, densidade de tela, orientação, etc.).
* **Gradle**: ferramenta de automação de build com configuração por projeto e por módulo.

## :books: **Referências**

1. LECHETA, R. _Google Android: Aprenda a criar aplicações para dispositivos móveis com o Android SDK_. Novatec, 4ª ed., 2015.
2. História do Android: [https://www.android.com/intl/pt-BR\_br/history](https://www.android.com/intl/pt-BR_br/history)
3. Fundamentos: [https://developer.android.com/guide/components/fundamentals](https://developer.android.com/guide/components/fundamentals)
4. Arquitetura: [https://developer.android.com/guide/platform](https://developer.android.com/guide/platform)

