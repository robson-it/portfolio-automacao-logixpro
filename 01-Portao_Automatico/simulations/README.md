
## :video_camera: Vídeo simulação do portão automático:

https://github.com/user-attachments/assets/b111c6a8-0794-41f9-8b7d-9244a2ea391a


🎯 Testes realizados na simulação:

- Abertura do portão através da botoeira OPEN.
- Fechamento do portão através da botoeira CLOSE.
- Tentativa de fechamento do portão enquanto em processo de abertura, possibilitando verificar o intertravamento.
- Tentativa de abertura do portão enquanto em processo de fechamento, possibilitando verificar o intertravamento.
- Parada total do sistema através da botoeira STOP.
- Verificação dos sinaleiros OPEN -> Portão aberto, SHUT -> Portão fechado e AJAR -> entreaberto.
- Verificação da lógica de selo, onde foi utilizado um contato NO (Normal Open) de cada motor, para manter a linha energizada.
- Verificação da lógica de intertravamento, onde foi utilizado um contato NC (Normal Close) de cada motor "cruzados", impedindo o acionamento simultâneo.


<img width="850" height="511" alt="Lógica_Ladder" src="https://github.com/user-attachments/assets/9e0b31cd-1d8f-44e9-bf94-2858c445b67e" />
