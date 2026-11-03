# 🚧 Portão Automático

### 📌 Visão Geral

Este projeto consiste no desenvolvimento de um sistema automatizado para controle de abertura e fechamento de um portão, utilizando programação Ladder (LD) em um Controlador Lógico Programável (CLP).

O sistema utiliza dois acionamentos independentes, destinados aos movimentos de abertura e fechamento, além de sensores de fim de curso para identificar os limites de movimentação do portão.

A lógica foi desenvolvida no ambiente LogixPro, aplicando conceitos de comandos elétricos e automação industrial.

### 🎯 Contexto de Aplicação

Em instalações industriais, centros logísticos e áreas de acesso controlado, portões são utilizados para controlar a entrada e saída de veículos e pessoas.

A operação manual desses dispositivos pode exigir intervenção constante de operadores, tornando o processo menos eficiente.

A automatização desse mecanismo permite controlar os movimentos do portão por meio de comandos elétricos e dispositivos de monitoramento, proporcionando maior praticidade e organização operacional.

### 🎯 Objetivo do Projeto

Desenvolver uma lógica de controle para automatizar a abertura e o fechamento de um portão, utilizando recursos de programação Ladder.

O projeto tem como objetivos:

- Implementar comandos independentes de abertura e fechamento.
- Controlar os acionamentos por meio de saídas distintas do CLP.
- Utilizar sensores de fim de curso para identificar as posições extremas.
- Aplicar circuitos de selo para manter os acionamentos ativos.
- Implementar intertravamento para impedir comandos simultâneos de abertura e fechamento.
- Simular e validar o funcionamento da lógica desenvolvida.

### ⚙️ Arquitetura do Sistema
 
O sistema é composto por dispositivos de comando, sensores de posicionamento e elementos de acionamento.

| Elemento: _____________________________ | Função: ______________________________________ | \
| CLP_____________________________________: Processamento da lógica de controle \
| Botão de abertura______________________: Solicita a abertura do portão \
| Botão de fechamento__________________: Solicita o fechamento do portão \
| Botão de parada________________________: Interrompe o funcionamento do sistema \
| Sensor de fim de curso aberto_________: Identifica o limite de abertura \
| Sensor de fim de curso fechado________: Identifica o limite de fechamento \
| Saída de abertura_______________________: Acionamento responsável pela abertura \
| Saída de fechamento___________________: Acionamento responsável pelo fechamento \
| Lâmpada Shut__________________________: Indica o fechamento completo do portão \
| Lâmpada Open_________________________: Indica a abertura completa do portão \
| Lâmpada Ajar___________________________: Indica o portão entreaberto 

### 🧠 Lógica de Controle

A programação foi desenvolvida utilizando a linguagem Ladder (LD), explorando recursos fundamentais de automação e comandos elétricos.

1. Comando de abertura

Ao receber o comando de abertura, o CLP verifica as condições necessárias para permitir o acionamento.

O circuito de selo mantém o comando ativo durante o movimento, até que a condição de parada seja atingida pelo sensor de fim de curso correspondente ou o botão de STOP seja acionado.

2. Comando de fechamento

O funcionamento segue uma lógica equivalente à abertura, utilizando um acionamento independente.

O movimento é mantido por meio do circuito de selo até que o sensor de fim de curso de fechamento identifique a posição final ou o botão de STOP seja acionado.

3. Intertravamento

Foi implementado um sistema de intertravamento lógico entre os comandos de abertura e fechamento.

Essa condição impede que os dois acionamentos sejam comandados simultaneamente, evitando solicitações conflitantes de movimentação.

4. Sensores de fim de curso

Os sensores monitoram os limites de movimentação do portão, permitindo interromper o acionamento correspondente quando a posição final é alcançada.

### 🔌 Recursos de Programação Aplicados

- Linguagem Ladder (LD).
- Circuitos de selo.
- Intertravamento lógico.
- Comandos independentes de acionamento.
- Monitoramento por entradas digitais.
- Controle de saídas digitais.
- Sensores de fim de curso.
- Sinalização do funcionamento por sinaleiros.

### 📐 Diagramas Elétricos

Esta seção reúne a documentação elétrica do projeto, permitindo visualizar a estrutura dos circuitos e a relação entre os dispositivos de comando e acionamento.

- Diagrama de comando elétrico.
- Diagrama de potência, conforme a arquitetura de acionamento adotada.

Os diagramas estarão disponíveis no diretório "docs/".

### 🧪 Simulação e Validação

O projeto foi desenvolvido e testado utilizando o ambiente LogixPro.

Durante a simulação, podem ser verificadas as seguintes condições:

- Acionamento do comando de abertura.
- Acionamento do comando de fechamento.
- Retenção dos comandos por meio dos circuitos de selo.
- Interrupção dos movimentos pelos sensores de fim de curso.
- Funcionamento do intertravamento entre os acionamentos.

Os vídeos e demais evidências de funcionamento estarão disponíveis no diretório "simulation/".

### 📁 Estrutura do Projeto

portao-automatico/ \
│ \
├── README.md \
│ \
├── docs/ \
│   ├── diagrama-comando \
│   └── diagrama-potencia \
│ \
├── plc/ \
│   └── programa-ladder \
│ \
├── simulation/ \
│   └── videos-e-evidencias 

### 🚀 Possíveis Melhorias

Como possibilidades de evolução, o sistema poderá receber:

- Detecção de obstáculos durante a movimentação.
- Sinalização visual e sonora.
- Monitoramento de falhas nos acionamentos.
- Integração com sistemas de controle de acesso.
- Implementação de parada de emergência.

### 🛠️ Tecnologias e Ferramentas

- Linguagem: Ladder (LD).
- Ambiente de desenvolvimento e simulação: LogixPro.
- Controlador: CLP simulado no ambiente LogixPro.

### 👨‍💻 Autor

Robson Alves Rocha

Projeto desenvolvido como parte do portfólio de Automação Industrial, com foco na aplicação prática de conceitos de programação de CLPs, comandos elétricos e controle de sistemas automatizados.
