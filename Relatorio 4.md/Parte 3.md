# Relatório 4 -  Transistores do tipo MOS

## Parte 3 - Espelho de corrente com transistores do tipo NMOS:

#### Objetivo:

1 - Simular e explicar o funcionamento do circuito abaixo comparando as corrente ID1 e ID2:

![nome](/relatorio_eletronica_1/circ3.png)

2 - Variar a resistência R2 e traçar a curva ID2 x V2

3 - Obter o valor máximo de R2 para o espelho de corrente funcionar corretamente

4 - Comparar os resultados simulados com os teóricos.

#### Funcionamento do circuito.
O circuito espelho de corrente com transistor NMOS possui 2 correntes denominadas ID1 e ID2, onde ID1 pode ser chamada de corrente de referência. Essa corrente de referência é calculada subtraindo a tensão porta-fonte da tensão de alimentação e dividindo pelo resistor entre a alimentação e a tensão porta-fonte.
A corrente que passa por Q1 gera uma tensão e essa tensão polariza o Q2, porém, há a necessidade de que Q1 seja igual a Q2, isto é, os transistores precisam ter as mesmas características físicas para este circuito funcionar corretamente como espelho de corrente. No caso, o Q1 age como um conversor de corrente para a tensão enquanto Q2 age como um conversor de tensão para a corrente.

#### Valores de VGS e Rmáximo

![nome](/relatorio_eletronica_1/contasresist.png)

Como o valor de VGS'' é menor que Vt foi utilizado o VGS' para a conta de IREF, pois é necessário um valor maior que Vt para ele continuar operando.


O valor de Resistência máximo é de aproximadamente 1023 ohms.

#### Valores de VGS e Rmáximo simulados

![nome](/relatorio_eletronica_1/simuladios.png)

Como a corrente I(R2) é a mesma da corrente de IREF calculado anteriormente temos que o resultado do simulado é muito próximo do resultado do teórico.

R2 = VCC - VT/ID2

R2 = 9,99 - 2,154/0,00763875

R2 = 1025,82 ohms.
