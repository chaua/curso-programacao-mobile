---
description: >-
  Comparação entre apps nativos, híbridos, web e PWA, com foco em usos e
  vantagens.
---

# 🧩 Aula 04 - Tipos de aplicativos móveis

{% hint style="info" %}
## Material da aula

* [Slides](slides/Aula04%20-%20Tipos%20de%20aplicativos.pdf)
{% endhint %}

## **Introdução**

A escolha do tipo de aplicativo é uma das decisões mais importantes no desenvolvimento mobile. Ela impacta diretamente a experiência do usuário, o desempenho da aplicação, o custo e o tempo de desenvolvimento, bem como o nível de acesso aos recursos do dispositivo. Esta aula apresenta os principais tipos de aplicativos móveis — nativos, web, híbridos e PWAs —, suas características, vantagens, limitações e exemplos práticos de uso.

## **1. Aplicativos Nativos**

São desenvolvidos exclusivamente para um sistema operacional (Android ou iOS) utilizando linguagens específicas:

* **Android**: Java, Kotlin.
* **iOS**: Swift, Objective-C.
* Utilizam ferramentas como Android Studio e Xcode.

**Vantagens:**

* Alto desempenho e fluidez.
* Acesso completo ao hardware (GPS, câmera, sensores).
* Melhor experiência de usuário e segurança.

**Desvantagens:**

* Custo e tempo de desenvolvimento elevados.
* Exigem equipes separadas para cada plataforma.
* Atualizações independentes por sistema.

## **2. Aplicativos Web (Web Apps)**

Executados diretamente em navegadores, sem necessidade de instalação:

* Desenvolvidos com HTML, CSS e JavaScript.
* Utilizam frameworks como React.js, Angular e Vue.js.

**Vantagens:**

* Acesso por URL em qualquer dispositivo.
* Um único código para todas as plataformas.
* Atualizações automáticas.

**Desvantagens:**

* Dependem da conexão com a internet.
* Acesso limitado a recursos do dispositivo.
* Desempenho inferior aos nativos.

## **3. Aplicativos Híbridos**

Combinam elementos de apps nativos e web, rodando dentro de um container nativo:

* Desenvolvidos com tecnologias web mais frameworks como React Native, Flutter, Ionic.

**Vantagens:**

* Compartilham código entre Android e iOS.
* Reduzem custo e tempo de desenvolvimento.
* Acesso parcial a recursos do dispositivo.

**Desvantagens:**

* Desempenho inferior aos nativos.
* Dependência de terceiros (frameworks).
* Limitações na personalização de UI.

## **4. Progressive Web Apps (PWAs)**

São Web Apps que simulam o comportamento de aplicativos nativos:

* Utilizam tecnologias como Service Workers e Web App Manifest.

**Vantagens:**

* Podem ser adicionados à tela inicial do dispositivo.
* Funcionam offline.
* Consomem menos dados.
* Não exigem instalação via lojas de aplicativos.

**Desvantagens:**

* Integração limitada com recursos do dispositivo.
* Restrição de funcionalidades, especialmente no iOS.
* Dificuldade de aceitação nas app stores.

## **5. Comparação entre Tipos de Aplicativos**

<table><thead><tr><th width="247.5">Característica</th><th width="113">Nativo</th><th width="111.5">Híbrido</th><th width="125.5">Web App</th><th>PWA</th></tr></thead><tbody><tr><td>Performance</td><td>Alta</td><td>Média</td><td>Baixa</td><td>Média</td></tr><tr><td>Acesso a recursos</td><td>Total</td><td>Parcial</td><td>Limitado</td><td>Parcial</td></tr><tr><td>Custo de desenvolvimento</td><td>Alto</td><td>Médio</td><td>Baixo</td><td>Baixo</td></tr><tr><td>Necessita instalação</td><td>Sim</td><td>Sim</td><td>Não</td><td>Opcional</td></tr><tr><td>Exemplo</td><td>WhatsApp</td><td>Instagram</td><td>Google Docs</td><td>Twitter Lite</td></tr></tbody></table>

## **6. Qual escolher?**

A escolha depende das necessidades específicas do projeto:

* **App nativo**: quando a performance e o acesso ao hardware são cruciais.
* **Web app**: para soluções simples e universais, com menor custo.
* **App híbrido**: para projetos que buscam equilíbrio entre custo e funcionalidade.
* **PWA**: quando se deseja acessibilidade, leveza e funcionamento offline.

