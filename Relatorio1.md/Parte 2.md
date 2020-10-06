# Relatório 1 - AmpOp

## Parte 2: Amplificador Inversor

#### Objetivo:

Medir o ganho de um amplificador inversor e verificar o efeito da saturação

#### Experimento:

Utilizar o Amplificador operacional LM324N e o TL082 para montar dois amplificadores inversores utilizando um resistor de realimentação de 20 kΩ e uma resistência de entrada de 2kΩ.
Utilizar uma alimentação simétrica de +12V e -12V.

#### Procedimento:

1 - Simular o circuito utilizando como tensão de entrada um sinal senoidal com 0,5 Vp e 1kHz.

2 - Mostrar os resultados da tensão de saída.

3 - Verificar o valor do ganho obtido.

4 - Aumentar o valor da tensão de entrada e analisar para qual valor da tensão de entrada ocorre a saturação do sinal.

5 - Verificar qual o valor da queda de tensão com relação à tensão de alimentação.

6 - Resultados.

#### Circuito utilizando o AmpOp LM324N


![nome](/relatorio_eletronica_1/circuitolmparte2.png)

#### Ganho da tensão entrada:
Para saber por quanto a tensão de entrada será multiplicada, calcula-se o ganho da tensão de entrada.

![nome](/relatorio_eletronica_1/ganho2.png)

#### Tensão de Entrada e de saída LM324N:

![nome](/relatorio_eletronica_1/entradaesaidaparte2.png)


#### Circuito utilizando o AmpOp TL082

![nome](/relatorio_eletronica_1/TL082.png)

#### Ganho da tensão entrada:
Como o circuito apresenta as mesmas características o ganho será o mesmo do circuito anterior já calculado.

#### Tensão de Entrada e de saída TL082:

![nome](/relatorio_eletronica_1/entradaesaidatl082.png)

### Análise de saturação

Após analisarmos a tensão de entrada e de saída dos respectivos circuitos simulados, iremos aumentar lentamente a tensão de entrada para verificarmos a ocorrência da saturação do sinal.


#### Análise de saturação Circuito LM324N:

![nome](/relatorio_eletronica_1/saturaçaolm3241.png)

Após aumentarmos lentamente a tensão de entrada do circuito percebe-se a saturação quando a tensão de entrada recebe o valor de 1.08V, porém, apenas a parte positiva da onda.

Como o AmpOp não suporta uma tensão maior que a tensão de alimentação, que nesse caso é de 12V e ele acaba saturando em 10,77V a queda de tensão será dada por 12V - 10,77V = 1,23V.

![nome](/relatorio_eletronica_1/saturacaaaaao.png)

Após um aumento de 0,07V na tensão de entrada a parte negativa acabou saturando também, ou seja, quando o sinal de entrada atingiu o valor de 1,14V tanto a parte positiva como a negativa saturaram.

Como ainda temos uma tensão de alimentação de 12V, e a parte negativa satura em -11,32V teremos uma queda de tensão de -12V - (-11,32V) = -0,68V.

#### Análise de saturação Circuito TL082:

![nome](/relatorio_eletronica_1/saturaçaotl082.png)

![nome](/relatorio_eletronica_1/negativasatur.png)

Após aumentarmos lentamente a tensão de entrada, foi verificado uma saturação ao atingir um valor de 1,06V na parte positiva e negativa.
Como a saturação ocorreu nos pontos de tensão de 10,37V e de -10,37V então o valor da queda de tensão será +/- 12V - (+/- 10,37) = +/-1,63V


### Resultados

Quando efetuamos o calculo do ganho, fica visível na onda da tensão de entrada comparando com a tensão de saída a diferença entre os valores, nesse caso, 10x maior. A tensão de entrada com um valor de 500mV e a tensão de saída de 5V.
Ambos os circuitos simulados apresentavam uma tensão de alimentação de 12V, ou seja, sabemos que ele irá saturar em valores maiores que a tensão de alimentação. No caso do circuito LM324N houve uma diferença nos valores de saturação positiva e negativa, a positiva sendo em 10,77V e a negativa em -11,32, tendo valores de queda de tensão de 1,23V e -0,68V respectivamente. No caso do circuito do TL082 a saturação positiva e negativa apresentaram mesmo valor de +1,63V e -1,63V.
