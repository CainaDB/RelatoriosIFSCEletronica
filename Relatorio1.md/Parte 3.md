# Relatório 1 - AmpOp

### Parte 3: Amplificador Não-Inversor

#### Objetivo:

Medir o ganho de um amplificador não-inversor e verificar o efeito da saturação

#### Experimento:

Utilizar um Amp.OP. LM324N e um TL082 e montar dois amplificadores não-inversores. Utilizando um resistor de realimentação com valor 20 kΩ e o outro resistor igual à 2kΩ.
Utilize a alimentação simétrica de +/-12V.

#### Procedimento:

1 - Simular o circuito utilizando como tensão de entrada um sinal senoidal com 0,5 Vp e 1kHz.

2 - Mostrar os resultados da tensão de saída.

3 - Analisar o valor do ganho obtido.

4 - Aumentar o valor da tensão de entrada e verificar para qual valor da tensão de entrada ocorre a saturação do sinal.

5 - Verificar qual o valor da queda de tensão com relação à tensão de alimentação.

6 - Resultados.

#### Circuito utilizando o AmpOp LM324N

![nome](/relatorio_eletronica_1/ninversorlm324.png)

#### Ganho da tensão entrada:
Para saber por quanto a tensão de entrada será multiplicada, calcula-se o ganho da tensão de entrada.


#### Tensão de Entrada e de saída LM324N:

![nome](/relatorio_eletronica_1/ninversorlm3241.png)

A tensão de saída é de aproximadamente 5,51V

#### Circuito utilizando o AmpOp TL082

![nome](/relatorio_eletronica_1/tl082ninversor.png)

A tensão de saída é de aproximadamente 5,49V

#### Tensão de Entrada e de saída TL082:

![nome](/relatorio_eletronica_1/ninversortl08.png)

### Análise de saturação

Após analisarmos a tensão de entrada e de saída dos respectivos circuitos simulados, iremos aumentar lentamente a tensão de entrada para verificarmos a ocorrência da saturação do sinal.

#### Análise de saturação Circuito LM324N:

![nome](/relatorio_eletronica_1/saturaçaoninversor.png)

Após o aumento gradativo da tensão de entrada percebe-se uma saturação na parte positiva quando o sinal de entrada atinge 0,99V. Como a tensão de alimentação é de 12V e o ponto de saturação foi de 10,77V temos uma queda de tensão de 1,23V

![nome](/relatorio_eletronica_1/ninversorsaturado.png)

Após a saturação da parte positiva, houve um aumento de 0,05V na tensão de entrada para saturar a parte negativa do circuito, com a mesma tensão de alimentação de 12V o ponto de saturação dessa vez foi em -11,33V, com isso, a queda de tensão será dada por -12V - (-11,33V) = -0,67V.


#### Análise de saturação Circuito TL082:

![nome](/relatorio_eletronica_1/saturadotl082.png)

![nome](/relatorio_eletronica_1/saturado22.png)

Após o aumento gradual da tensão de entrada houve saturação na parte positiva e negativa quando obtivemos o valor de 1,40V de entrada. Nesse caso, o valor de tensão no ponto de saturação foi de +/-10,47V, com isso, o valor de queda de tensão será de +/-12V - (+/-10,47V) = +/- 1,53V

### Resultados

Quando efetuamos o calculo do ganho, fica visível na onda da tensão de entrada comparando com a tensão de saída a diferença entre os valores, nesse caso, 11x maior. A tensão de entrada com um valor de 0,5V e a tensão de saída de 5,51V.
Ambos os circuitos simulados apresentavam uma tensão de alimentação de 12V, ou seja, sabemos que ele irá saturar em valores maiores que a tensão de alimentação. No caso do circuito LM324N houve uma diferença nos valores de saturação positiva e negativa, a positiva sendo em 10,77V e a negativa em -11,33V, tendo valores de queda de tensão de 1,23V e -0,67V respectivamente. No caso do circuito do TL082 a saturação positiva e negativa apresentaram mesmo valor de +1,53V e -1,53V.
