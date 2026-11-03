## :video_camera: Vídeo simulação do portão automático com temporizador para fechamento automatizado após o tempo determinado:

https://github.com/user-attachments/assets/a053f9ee-b4d7-4d0b-bf2d-b50f47bdb421

### 🎯 Testes realizados na simulação:

- Abertura do portão através da botoeira OPEN.
- Fechamento do portão através da botoeira CLOSE.
- Tentativa de fechamento do portão enquanto em processo de abertura, possibilitando verificar o intertravamento.
- Tentativa de abertura do portão enquanto em processo de fechamento, possibilitando verificar o intertravamento.
- Aguardo de tempo determinado com o portão aberto, para verificar o fechamento automático.
- Parada total do sistema através da botoeira STOP.
- Verificação dos sinaleiros OPEN -> Portão aberto, SHUT -> Portão fechado e AJAR -> entreaberto.
- Verificação da lógica de selo, onde foi utilizado um contato NO (Normal Open) de cada motor, para manter a linha energizada.
- Verificação da lógica de intertravamento, onde foi utilizado um contato NC (Normal Close) de cada motor "cruzados", impedindo o acionamento simultâneo.


### :computer: Screenshot do programa desenvolvido em Ladder:

<img width="1138" height="873" alt="Captura de tela 2026-11-03 154255" src="https://github.com/user-attachments/assets/1bfe34c0-c083-428d-9a24-66ea1474c3ea" />
