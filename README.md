## Fonte de Alimentação Regulada 12V com 7812

## 1. Descrição do Projeto

Este projeto apresenta o desenvolvimento de uma fonte de alimentação regulada de 12V, baseada no regulador linear 7812.
A fonte foi projetada e simulada utilizando o Proteus Design Suite, incluindo:

* Diagrama esquemático do circuito
* Projeto da placa de circuito impresso (PCB)
* Visualização tridimensional da placa

O circuito recebe uma tensão alternada (AC) proveniente de um transformador, realiza a retificação, passa por um processo de filtragem e, por fim, fornece uma tensão contínua estável de 12V (DC) na saída.

====================================================================================================================================================================
## 2. Finalidade

O objetivo deste projeto é demonstrar, de forma prática, o funcionamento de uma fonte linear regulada, muito utilizada em circuitos eletrônicos para fornecer tensão contínua estável.

As etapas principais do funcionamento são:

* Conversão de tensão AC para DC
* Redução de ondulações na tensão
* Regulação da tensão de saída
* Indicação de funcionamento através de LED

==================================================================================================================================================================
## 3. Diagrama do Circuito
O esquemático apresenta todos os componentes eletrônicos utilizados e suas conexões, permitindo compreender o funcionamento completo da fonte.

<img width="1286" height="657" alt="Captura de tela 2026-03-10 220451" src="https://github.com/user-attachments/assets/429caeea-ef3c-48c4-a3a4-539d13463367" />

==================================================================================================================================================================
# 4. Lista de Componentes

| Componente | Função |
|------------|--------|
| J2 | Conector de entrada do transformador |
| BR1 | Ponte retificadora |
| C1 | Capacitor eletrolítico 1000µF |
| C2 | Capacitor cerâmico 100nF |
| U1 | Regulador de tensão 7812 |
| C3 | Capacitor cerâmico 100nF |
| R1 | Resistor 100Ω |
| D1 | LED indicador |
| J1 | Conector de saída |

==================================================================================================================================================================
## 5. Etapas de Funcionamento

Entrada de Energia

A alimentação do circuito é feita através do conector J2, ligado ao secundário de um transformador que reduz a tensão da rede elétrica para um nível adequado (exemplo: 12V AC).

==================================================================================================================================================================
## Processo de Retificação

A tensão alternada proveniente do transformador é aplicada à ponte retificadora (BR1).

Essa ponte é formada por quatro diodos que convertem a corrente alternada em corrente contínua pulsante.

==================================================================================================================================================================
## Filtragem da Tensão

Após a retificação, a tensão ainda apresenta pequenas variações chamadas de ripple.

Para suavizar essas oscilações são utilizados:

* C1 (1000µF) – capacitor responsável pela filtragem principal
* C2 (100nF) – capacitor que reduz ruídos de alta frequência

==================================================================================================================================================================## Regulação da Tensão

A tensão filtrada é aplicada ao regulador 7812, que garante uma saída fixa de 12V DC.

O regulador possui três terminais:

| Pino | Função |
|------|--------|
| 1 | Entrada |
| 2 | Terra (GND) |
| 3 | Saída regulada |

O capacitor C3 (100nF) auxilia na estabilidade da saída.

==================================================================================================================================================================
## Indicador de Funcionamento

O LED (D1) indica quando a fonte está em operação.

O resistor R1 (100Ω) limita a corrente que passa pelo LED, evitando danos ao componente.

==================================================================================================================================================================
## Saída da Fonte

A tensão regulada é disponibilizada no conector J1, onde temos:

* +12V – tensão contínua regulada
* GND – referência de terra

Essa saída pode alimentar diferentes circuitos eletrônicos.

==================================================================================================================================================================
## 6. Projeto da Placa (PCB)

A placa foi projetada com dimensões aproximadas de:

## 80 mm x 40 mm

O layout foi organizado para:

* reduzir o tamanho das trilhas
* facilitar a montagem
* melhorar a organização dos componentes

<img width="1135" height="750" alt="PCB Layout" src="https://github.com/user-attachments/assets/1f2c2e02-58e3-4191-b0a6-7da8590cd385" />

==================================================================================================================================================================
## 7. Visualização 3D

A visualização tridimensional da placa permite observar como os componentes ficarão posicionados após a montagem.

## Vista superior

<img width="1226" height="700" alt="3D visualizer parte de cima" src="https://github.com/user-attachments/assets/5e367819-6dfd-4fbc-99c1-d591c72d45e1" />

## Vista inferior

<img width="1197" height="681" alt="3D visualizer parte de baixo" src="https://github.com/user-attachments/assets/d2b4ca7e-4149-4ae0-abb2-a948956141d0" />

==================================================================================================================================================================
## 8. Sequência de Operação da Fonte

O funcionamento completo ocorre da seguinte forma:

1. O transformador reduz a tensão da rede elétrica
2. A ponte retificadora converte AC em DC
3. O capacitor filtra a tensão
4. O regulador 7812 estabiliza em 12V
5. O LED indica funcionamento
6. A tensão regulada é disponibilizada na saída

==================================================================================================================================================================
## 9. Possíveis Aplicações

Fontes reguladas de 12V podem ser utilizadas em diversos projetos eletrônicos, como:

* Alimentação de placas Arduino
* Projetos de robótica
* Protótipos de sistemas embarcados
* Circuitos de sensores
* Pequenos dispositivos eletrônicos

==================================================================================================================================================================## 10. Ferramentas Utilizadas

O desenvolvimento do projeto foi realizado com o software:

## Proteus Design Suite

Módulos utilizados:

* ISIS – criação do esquemático
* ARES – desenvolvimento da PCB
* 3D Viewer – visualização tridimensional da placa

==================================================================================================================================================================## 11. Observação Técnica

Para que o regulador 7812 funcione corretamente, a tensão de entrada deve ser maior que a tensão de saída.

Normalmente é necessário ter entre 14V e 15V na entrada para garantir uma saída estável de 12V DC.

==================================================================================================================================================================## 12. Autor

Projeto desenvolvido para a disciplina de Sistemas Embarcados.

Autor: Jhonatan Negri
