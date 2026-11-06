## :video_camera: Vídeo simulação de um tanque batch com display para seleção de nível:




https://github.com/user-attachments/assets/9e508118-27d2-427a-a947-81adbe19d18d



### 🎯 Testes realizados na simulação:

- Funcionamento de duas bombas para encher um tanque
- Verificação do nível máximo ao encher o tanque, sem transbordar
- Verificação do nível do tanque através do display BCD, comparando com o valor selecionado no seletor BCD
- Acionamento de um mixer, para fazer a mistura dos fluídos e deixa-los homogêneos.
- Acionamento do heater para aquecimento do líquido até a temperatura definida no termostato, antes de dar vasão
- Acionamento da bomba de vasão, após a conclusão do processo de mistura e aquecimento
- Teste de parada do sistema através da botoeira STOP, foi definido que durante o enchimento do tanque a parada seria imediata, porém, após o enchimento do tanque e início do processo, se acionada a botoeira STOP, o sistema executa a parada apenas após finalizar a vasão do fluído.
- Foi definido que o tanque será enchido 50% pela bomba 1 e 50% pela bomba 2 e o limite será definido no seletor BCD. Caso o nível selecionado seja maior que a capacidade do tanque, o sensor alto faz a verificação, permitindo que o tanque encha até o seu limite sem transbordar. 


### :computer: Screenshot do programa desenvolvido em Ladder:

<img width="1041" height="2252" alt="Captura de tela 2026-11-06 170353" src="https://github.com/user-attachments/assets/aab9a240-fb5c-4a88-a5ce-053c38068927" />


