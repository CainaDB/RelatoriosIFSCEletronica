# Projeto Final

### Projeto Fonte Linear

#### Objetivo:

Integração dos blocos de uma fonte linear.

#### Procedimento:

O projeto da fonte linear será dividido em 3 partes, dentre elas:

Parte 1: Simulação do circuito e resposta aos questionamentos.

Parte 2: Dimensionamento dos componentes do circuito da fonte linear.

Parte 3: Adição do circuito de proteção de sobre corrente ao regulador linear.

#### Circuito proposto

![nome](/relatorio_eletronica_1/fonte1.png)

##### Qual relação entre a tensão de alimentação do AmpOp e a tensão de saída?

Comoa tensão do circuito com AmpOp não ultrapassa a sua tensão de alimentação, nesse caso, a tensão de saída é regulada pela tensão de alimentação do AmpOp, isto é, há uma limitação de tensão de saída pela tensão de alimentação do AmpOp.

##### O que devemos considerar para esse circuito operar como um LDO?

Um LDO (Low-Dropout) nada mais é que um regulador linear de baixa queda de tensão, eles são usados para fornecer uma tensão de alimentação estável independente da impedância da carga, variações de tensão de entrada, temperatura e tempo. A queda de tensão na saída necessita-se de um valor baixo, de 0,1V a 0,5V, com isso, temos que Vout = VZ[1+(R2/R3)] onde a tensão de saída dependerá da tensão de referência do diodo Zener conectado e a relação entre R2 e R3.
