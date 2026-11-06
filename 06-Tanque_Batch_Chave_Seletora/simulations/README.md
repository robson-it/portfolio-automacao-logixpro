## :video_camera: Vídeo simulação de um tanque batch com chave seletora para fluxo em duas bombas:

https://github.com/user-attachments/assets/1ab76073-ffe4-405a-a7de-1030b575bfd6


### 🎯 Testes realizados na simulação:

- Funcionamento de duas bombas para encher um tanque
- Verificação do nível máximo ao encher o tanque, sem transbordar
- Acionamento de um mixer, para fazer a mistura dos fluídos e deixa-los homogêneos.
- Acionamento do heater para aquecimento do líquido até a temperatura definida no termostato, antes de dar vasão
- Acionamento da bomba de vasão, após a conclusão do processo de mistura e aquecimento
- Teste de parada do sistema através da botoeira STOP, foi definido que durante o enchimento do tanque a parada seria imediata, porém, após o enchimento do tanque e início do processo, se acionada a botoeira STOP, o sistema executa a parada apenas após finalizar a vasão do fluído.
- Teste de chave seletora, para definir a quantidade de líquido que será bombeado pelas bombas 1 e 2. Ficando definido que a posição A divide em 50% para cada bomba, a posição B divide em 1/3 para a bomba 1 e 2/3 para a bomba 2 e a posição C divide em 1/5 para a bomba 1 e 4/5 para a bomba 2. 


### :computer: Screenshot do programa desenvolvido em Ladder:

<img width="1074" height="1969" alt="Captura de tela 2026-11-06 162313" src="https://github.com/user-attachments/assets/95beaffb-04a3-4144-9c02-7e084fb9e858" />

