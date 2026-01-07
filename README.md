# 🐍 SwiftSnake: Neon & Dynamic Speed Edition

Uma reinterpretação moderna e performática do clássico jogo da serpente, desenvolvida nativamente para iOS. Este projeto demonstra o uso de **SwiftUI** para interfaces declarativas e **Combine** para o gerenciamento de eventos de tempo e lógica de jogo reativa.



## 🚀 Funcionalidades Premium

- **Dificuldade Progressiva:** O motor do jogo utiliza um sistema de aceleração dinâmica. A cada ponto marcado, o `Timer` é recalibrado, aumentando a velocidade e o desafio em tempo real.
- **Controle Híbrido (Touch + Keyboard):**
    - **Gestos:** Implementação de `DragGesture` para controles intuitivos via deslize.
    - **Teclado:** Suporte nativo para as setas do teclado físico/notebook via `keyboardShortcut`, ideal para testes no simulador ou iPads.
- **Feedback Tátil (Haptic Engine):** Integração com `UIImpactFeedbackGenerator` para fornecer respostas físicas distintas ao coletar itens ou colidir.
- **Lógica de Direção Protegida:** Algoritmo que impede a inversão de movimento em 180º, evitando colisões acidentais imediatas.

## 🛠️ Stack Tecnológica

- **SwiftUI:** Construção de interface reativa e componentes de UI.
- **Combine:** Gerenciamento do ciclo de vida do jogo e publicação de eventos de tempo.
* **UIKit:** Utilizado especificamente para a camada de feedback tátil do sistema.



## 🏗️ Arquitetura e Boas Práticas

- **Gerenciamento de Estado:** Uso estratégico de `@State` para garantir sincronia total entre a lógica de movimentação e a renderização da grade.
- **Motor de Tempo (Timer):** Implementação de uma lógica de reinicialização de publicação (`updateTimer`) que cancela instâncias anteriores para evitar vazamentos de memória e sobreposição de batidas.
- **UI Responsiva:** Uso de `GeometryReader` e `aspectRatio` para garantir que o campo de jogo permaneça quadrado e centralizado em qualquer modelo de iPhone.

## 📦 Como Instalar e Rodar

1. Certifique-se de ter o **Xcode 15.0+** instalado.
2. Clone o repositório:
   ```bash
   git clone [https://github.com/seu-usuario/SwiftSnake-Neon.git](https://github.com/seu-usuario/SwiftSnake-Neon.git)
