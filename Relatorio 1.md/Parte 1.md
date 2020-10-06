# Relatório 1 - AmpOp

### Parte 1 - Seguidor de Tensão

#### Objetivo:

Analisar e explicar sobre o funcionamento de um circuito com características seguidor de tensão.

#### Experimento:

Utilizar um Amplificador Operacional do tipo LM324N e do tipo TL082 para montar dois circuitos com características de seguidor de tensão, com uma resistência de realimentação de 10 kΩ em cada um dos circuitos. Utilizar a alimentação simétrica de +/-12V.
#### Procedimento:
Simular o circuito com tensão de entrada um sinal senoidal com 0,5 Vp e 1kHz de frequência.
#### Circuito utilizando um AmpOp LM324N
Utilizando o software LTSpice foi montado o circuito:


![nome](/relatorio_eletronica_1/CIRCUITOLM324NIMAGEM.jpg)

#### Ganho da tensão entrada:
Para saber por quanto a tensão de entrada será multiplicada, calcula-se o ganho da tensão de entrada.

![nome](/relatorio_eletronica_1/ganho.png)

#### Tensão de Entrada:


![nome](/relatorio_eletronica_1/TENSAODEENTRADA.png)

#### Tensão de Saída:

![nome](/relatorio_eletronica_1/tensaodesaida.png)

#### Circuito utilizando um AmpOp TL082

![nome](/relatorio_eletronica_1/circuitotl.png)

#### Ganho da tensão entrada:
Como o resistor é de 10k e o circuito apresenta as mesmas características, o ganho será igual ao circuito anterior.

#### Tensão de Entrada:


![nome](/relatorio_eletronica_1/entradacircuito2.png)

#### Tensão de Saída:


![nome](/relatorio_eletronica_1/saidacirc2.png)

## Resultados
Com os dois circuitos montados e comparados, podemos perceber a característica principal de seguidor de tensão (Buffer), isto é, como o ganho de tensão é unitário entre os dois circuitos, a tensão de saída será igual a tensão de entrada.
