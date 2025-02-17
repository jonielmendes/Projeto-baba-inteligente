# 👶 Babá Inteligente com Raspberry Pi Pico W – Monitoramento de Som em Tempo Real

Este projeto implementa uma **Babá Eletrônica** utilizando a **BitDOG**. Ele monitora sons no ambiente e executa ações específicas, como exibir informações no display OLED e alertar por meio de LEDs RGB e um buzzer.

🎥 **Vídeo Demonstrativo:**  
[Assista ao vídeo aqui](https://youtu.be/4mMymLLoecw?si=KBtV-JhVfErgunnD)

## 📌 Descrição do Projeto

A Babá Eletrônica detecta sons e fornece feedback visual e auditivo sobre o estado do ambiente. O sistema é controlado por botões físicos que permitem ativar e desativar a detecção de som.

### Funcionalidades

- **Detecção de Som:** Identifica ruídos no ambiente com um microfone analógico.
- **Reprodução de Melodia:** Toca "Brilha, Brilha Estrelinha" no buzzer ao detectar som.
- **Indicadores Visuais:**
  - 🔵 **Azul:** Sistema aguardando ativação.
  - 🟢 **Verde:** Sistema ativo.
 
- **Controle por Botões:**
  - **Botão A:** Ativa o sistema.
  - **Botão B:** Desativa o sistema.
- **Display OLED:** Exibe mensagens sobre o status do sistema.

## 🛠 Requisitos

### 📌 Hardware Necessário

- Raspberry Pi Pico W
- Display OLED SSD1306
- Buzzer Passivo
- Microfone Analógico
- Botões (2 unidades)
- LED RGB
- Protoboard e Jumpers

### 💾 Software Necessário

- Raspberry Pi Pico SDK
- Biblioteca SSD1306
- **Ferramentas de Desenvolvimento:**
  - Visual Studio Code com extensões para C/C++ e Pico SDK
  - CMake para geração de builds

## 📂 Estrutura do Projeto

```
projeto-baba-inteligente/
├── CMakeLists.txt        # Configuração do CMake
├── display_oled.c        # Código principal
├── src/
│   ├── ssd1306.h        # Header do display OLED
│   ├── ssd1306.c        # Driver do display OLED
└── README.md            # Documentação do projeto
```

## 🚀 Como Usar

### 1️⃣ Configuração de Hardware

Conecte os componentes conforme descrito na seção de hardware.

### 2️⃣ Configuração de Software

Compile o código utilizando o CMake:
```sh
mkdir build && cd build
cmake ..
make
```

### 3️⃣ Upload para a Raspberry Pi Pico

- Conecte sua Pico W via USB enquanto pressiona o botão **BOOTSEL**.
- Solte o botão e uma unidade USB aparecerá no seu computador.
- Arraste e solte o arquivo `.uf2` gerado para a unidade.

## 📞 Contato

Para mais informações, entre em contato:

- **Nome:** Joniel Mendes
- **Email:** jonielmendes237@gmail.com



