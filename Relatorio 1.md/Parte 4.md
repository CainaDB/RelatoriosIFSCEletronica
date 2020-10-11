# Relatório 1 - AmpOp

### Parte 4 - Amplificador Subtrator

#### Objetivo:

Verificar as não idealidades dos AmpOps aplicadas em um circuito subtrator.

#### Experimento:

Utilizando um Amp.OP. Lm324N e o TL082 montar dois amplificadores subtratores.
Usar o resistor de realimentação com valor 510kΩ e ganho igual á 10V/V.
Utilizar a alimentação simétrica de +/-12V. (limite a corrente em 0,05A).

#### Procedimento:
1 - Simular o circuitos abaixo

![nome](/relatorio_eletronica_1/figura1.png)


2 - Compare os resultados para o LM324N e para TL082.

3 - Caso a fonte V1 tenha o valor igual á 0(zero)V, qual o valor da tensão de saída, para ambos os circuitos? Explique.

4 - Caso o seja alterado para o circuito abaixo, existe alguma variação na saída? Explicar.

![nome](/relatorio_eletronica_1/figura2.png)

5 - Justificar as dissimilaridades encontradas utilizando os dados do datasheet.


### Circuitos Simulados

#### Utilizando LM324N

![nome](/relatorio_eletronica_1/circsimulado1.png)

###### Tensão de saída utilizando 12V de tensão de Entrada

![nome](/relatorio_eletronica_1/circ1lm.png)

Obtemos um valor de tensão de saída de aproximadamente 130,01mV

###### Tensão de saída utilizando 0V de tensão de Entrada

![nome](/relatorio_eletronica_1/utilizandovin0.png)

Obtemos um valor de tensão de saída de aproximadamente 31,43mV

##### Após acrescentarmos um resistor em serie de 620 Ohms

###### Tensão de saída utilizando 12V de tensão de Entrada

![nome](/relatorio_eletronica_1/maisumres.png)

Obtemos um valor de tensão de saída de aproximadamente 97,14mV

###### Tensão de saída utilizando 0V de tensão de Entrada

![nome](/relatorio_eletronica_1/maisumres1.png)

Obtemos um valor de tensão de saída de aproximadamente 31,43mV

#### Utilizando TL082

![nome](/relatorio_eletronica_1/tl.png)

###### Tensão de saída utilizando 12V de tensão de Entrada

![nome](/relatorio_eletronica_1/utiliz.png)

Obtemos um valor de tensão de saída de aproximadamente 95,14mV

###### Tensão de saída utilizando 0V de tensão de Entrada

![nome](/relatorio_eletronica_1/utili.png)

Obtemos um valor de tensão de saída de aproximadamente 120,67uV

##### Após acrescentarmos um resistor em serie de 620 Ohms

###### Tensão de saída utilizando 12V de tensão de Entrada

![nome](/relatorio_eletronica_1/acres.png)

Obtemos um valor de tensão de saída de aproximadamente 63,46V

###### Tensão de saída utilizando 0V de tensão de Entrada

![nome](/relatorio_eletronica_1/acre.png)

Obtemos um valor de tensão de saída de aproximadamente 120,67uV

### Resultados e conclusões.
