# 🥁 Java BeatBox - Use a Cabeça!

Este projeto é uma implementação do famoso **BeatBox** apresentado no livro **Use a Cabeça! Java (2ª ou 3ª Edição)**. Trata-se de uma aplicação que combina manipulação de áudio MIDI, interfaces gráficas com Swing e comunicação via Sockets (TCP/IP).

---

## 🚀 Funcionalidades

O BeatBox permite que você crie ritmos musicais de forma visual:
* **Grade de Sequenciamento:** 16 instrumentos diferentes em 16 batidas (beats).
* **Sons MIDI:** Utiliza a biblioteca `javax.sound.midi` para gerar sons de percussão reais.
* **Controle de Tempo:** Ajuste a velocidade da batida em tempo real através dos botões de BPM.
* **Networking (Chat & Ritmos):** Envie suas sequências rítmicas para outros usuários conectados ao servidor e veja o que eles estão tocando.

## 🛠️ Tecnologias Utilizadas

* **Java SE:** Linguagem principal.
* **Swing & AWT:** Para a construção da interface gráfica (GUI).
* **Java MIDI API:** Para a síntese de som e sequenciamento de eventos musicais.
* **Java Networking (Sockets):** Para a comunicação entre o `BeatBoxClient` e o `MusicServer`.
* **Serialização:** Para salvar e enviar os padrões de batida (objetos) pela rede.

## 📦 Como Executar

### 1. Pré-requisitos
* Java JDK 8 ou superior instalado e configurado no PATH.

### 2. Rodar o Servidor (Opcional - Para funções de rede)
Para que os usuários possam trocar mensagens e batidas, o servidor deve estar rodando primeiro:
```bash
javac MusicServer.java
java MusicServer
