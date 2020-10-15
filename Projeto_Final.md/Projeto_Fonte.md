# Projeto Final

## Projeto Fonte Linear

### Objetivo:

Integração dos blocos de uma fonte linear.

### Procedimento:

O projeto da fonte linear será dividido em 3 partes, dentre elas:

Parte 1: Circuito proposto e resposta aos questionamentos.

Parte 2: Simulação do circuito e dimensionamento dos componentes do circuito da fonte linear.

Parte 3: Adição do circuito de proteção de sobre corrente ao regulador linear.

## Parte 1: Circuito proposto e resposta aos questionamentos.

### Circuito proposto

![nome](/relatorio_eletronica_1/fonte1.png)

#### Qual relação entre a tensão de alimentação do AmpOp e a tensão de saída?

Comoa tensão do circuito com AmpOp não ultrapassa a sua tensão de alimentação, nesse caso, a tensão de saída é regulada pela tensão de alimentação do AmpOp, isto é, há uma limitação de tensão de saída pela tensão de alimentação do AmpOp.

#### O que devemos considerar para esse circuito operar como um LDO?

Um LDO (Low-Dropout) nada mais é que um regulador linear de baixa queda de tensão, eles são usados para fornecer uma tensão de alimentação estável independente da impedância da carga, variações de tensão de entrada, temperatura e tempo. A queda de tensão na saída necessita-se de um valor baixo, de 0,1V a 0,5V, com isso, temos que Vout = VZ[1+(R2/R3)] onde a tensão de saída dependerá da tensão de referência do diodo Zener conectado e a relação entre R2 e R3.

#### Como obter as tensões de alimentação para o AmpOp (VCC e VEE)?

Os valores das tensões de alimentação dos AmpOps estão disponíveis em seu Datasheet. Utilizando um dobrador de tensão alimentando a entrada VCC e a entrada VEE ligada ao terra você consegue fazer a alimentação correta para o circuito.


#### Utilizando o circuito dobrador de tensão, qual valor de VCC você obtêm para um sinal Vin+ de 12Vrms? Quais problemas apresentam esse circuito? Podemos melhorar?

Na parte 1 do relatório 3 foi visto que a tensão de VCC era de 32,54V, porém, se adicionarmos uma nova carga à saída VCC de resultado tem seu ripple aumentado, para diminuir esse ripple resultante se utiliza de um circuito regulador do tipo serie conectado após o circuito dobrador de tensão.

### Projetando a fonte

![nome](/relatorio_eletronica_1/blocofonte.png)

Para a fonte ser concluída, precisamos nos ater a construção de cada um desses blocos que como resultado final temos a fonte linear.

Especificações da fonte:

AmpOp LM324

MOSFET IRF540

Vout = 15V

Vin+ = 12Vrms

Iout = 1A

Tensão de ripple = 1V

Queda de tensão nos diodos = 0,7V

#### Primeiro e Segundo bloco

![nome](/relatorio_eletronica_1/simuladson.png)

Nessa simulação foi montado os dois primeiros blocos da fonte linear, referentes ao Transformador e ao Circuito Retificador

Para o circuito retificador será utilizado o do tipo onda completa com transformador em derivação, pois se fosse utilizado o sem ponto de derivação a queda de tensão seria 2x maior do que a usual de 0.7V. Com isso, temos um valor de tensão de pico de 16,3V na qual será utilizada um resistor de 16,3 Ohms para obtermos uma corrente máxima de 1A.

![nome](/relatorio_eletronica_1/voutvin.png)

Nesta simulação temos que Vin+ é de aproximadamente 16,95V e Vout é de aproximadamente 16.06V.

Especificações:

Vin+ = 12Vrms

Tensão de Ripple (pós retificador) = 1V

I carga = 1,1A

![nome](/relatorio_eletronica_1/capacifiltro.png)


![nome](/relatorio_eletronica_1/comcapa.png)

#### Sinal de tensão de saída (Vout)

![nome](/relatorio_eletronica_1/ripleson.png)

![nome](/relatorio_eletronica_1/rip.png)

Após adicionarmos o capacitor calculado de 9,17mF obtemos uma tensão de ripple de 0,72V menor que 1V como desejado.

#### Dobrador de tensão para a alimentação do AmpOp

Para alimentar o AmpOp com o circuito dobrador de tensão é necessário dimensionar o mesmo. Como foi visto anteriormente, utilizando 12Vrms a tensão de saída do circuito dobrador é de 32,54V, com um ripple de 10% e corrente de alimentação dos AmpOps de 0,1A foi dimensionado o circuito dobrador de tensão.

Foi utilizado o Diodo Zener UDZV27B de 27V da ROHM 5mA e um transistor 2N3904 da NXP.

![nome](/relatorio_eletronica_1/capaci1.png)

![nome](/relatorio_eletronica_1/dobradorr.png)

#### Tensão de saída do dobrador.

![nome](/relatorio_eletronica_1/dobrador.png)

A tensão VCC obteve um valor de 26,86V

### Circuito Regulador

Para o cálculo do resistor de zener foi utilizado a mesma fórmula do cálculo anterior porém com os respectivos valores.
Para os resistores do regulador foi calculado que o valor de R3 é metade do valor de R4 pela relação R3/R4=0,5 com isso foi utilizado para o regulador R3=10k e R4=20k.
Foi utilizado o Diodo zener UDZV10B (o mesmo usado para o dobrador porém com outra tensão no valor de 10V e 5mA), um transistor IRF540 da fabricante Vishay e o mesmo AmpOp utilizado em relatórios anteriores da ON Semiconductor.

![nome](/relatorio_eletronica_1/capaci2.png)

![nome](/relatorio_eletronica_1/regulador1.png)

#### Tensão de saída do regulador.

![nome](/relatorio_eletronica_1/consta.png)

Enquanto a carga não elevar a corrente para acima de 1A, isto é, valores de carga abaixo de 15 Ohms a fonte após o tempo de 34ms estará constante tendo um valor próximo de 15V.

#### Tensão de Ripple do regulador.

![nome](/relatorio_eletronica_1/ripleregulador1.png)

A tensão de ripple foi de aproximadamente 2mV.












## Parte 2: Dimensionamento dos componentes do circuito da fonte linear e simulação do circuito.
