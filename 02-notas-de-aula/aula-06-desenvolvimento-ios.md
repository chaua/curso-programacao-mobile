---
description: Introdução ao desenvolvimento de aplicativos iOS.
---

# 🍎 Aula 06 - Desenvolvimento iOS

{% hint style="info" %}
## Material da aula

* [Slides](slides/Aula06%20-%20Desenvolvimento%20iOS.pdf)
{% endhint %}

## **Introdução**

O iOS é o sistema operacional móvel da Apple, conhecido por seu alto desempenho, segurança, fluidez e padronização de design. Exclusivo para dispositivos da marca, como iPhone e iPad, o iOS representa uma plataforma altamente lucrativa e com usuários fiéis. Esta aula aborda desde sua evolução histórica e arquitetura até os aspectos técnicos e o ambiente de desenvolvimento.

## **1. Histórico do iOS**

* **2007**: Lançamento com o primeiro iPhone, sem App Store.
* **2008**: App Store e SDK para terceiros.
* **2014**: Introdução da linguagem Swift.
* **2019 em diante**: SwiftUI, widgets, foco em privacidade, inteligência artificial e automações.

## **2. Arquitetura do iOS**

Composta por quatro camadas principais:

* **Cocoa Touch**: UIKit, SwiftUI, ARKit.
* **Media**: AVFoundation, Core Animation.
* **Core Services**: CoreData, CloudKit, Foundation.
* **Core OS**: Kernel, segurança, drivers.

Baseado no sistema UNIX (Darwin), herdado do macOS, o iOS oferece forte estabilidade e segurança.

## **3. Ferramentas e Linguagens**

* **Linguagens**: Swift (moderna e principal) e Objective-C (legado).
* **Ferramentas**:
  * **Xcode**: IDE oficial da Apple.
  * **Swift Playgrounds**: ideal para iniciantes.
  * **Instruments**: análise de performance.
  * **TestFlight**: testes beta com usuários.

## **5. Ambiente de Desenvolvimento**

* **Xcode**: editor, simulador, debugger e designer de interface.
* Projeto pode ser iniciado com SwiftUI ou UIKit.
* Organização dos arquivos:
  * `HelloWorldApp.swift` (entrada)
  * `ContentView.swift` (interface)
  * `Assets.xcassets` (recursos visuais)
  * `Info.plist` (configurações)

## **6. Ciclo de Vida de um App iOS**

### UIKit

* Estados: Not Running, Inactive, Active, Background, Suspended.
* Controlado via `UIApplicationDelegate`.

### SwiftUI

* Abstrai o ciclo de vida usando `@Environment(\.scenePhase)`.

## :books: **Referências**

* Apple Developer Portal: [https://developer.apple.com](https://developer.apple.com)

