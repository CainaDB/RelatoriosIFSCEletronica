# Relatório 2 - Diodos

### Parte 1: Circuito Retificador de Meia Onda

#### Experimento:

Montar um circuito retificador de meia onda utilizando resistores de 270Ω.
Utilizar capacitores de 330μF e 2200μF.

#### Procedimento:

1 - Simular o circuito do retificador de meia onda, inicialmente sem capacitor e registrar os valores da tensão de pico, eficaz e média, valor da máxima tensão reversa e a corrente sobre os diodos em uma tabela.

2 - Conectar um capacitor de 330μF e anotar os valores solicitados.

3 - Substituir o capacitor de 330μF por um de 2200μF, observar o formato da onda da tensão de saída e anotar os valores de solicitados.

4 - Responder o que são resistores shunt e como determinar o valor do resistor para o circuito.

5- Resultados.

#### Circuito retificador de meia onda sem capacitor:

![nome](/relatorio_eletronica_1/circuitomontado.png)

#### Amplitude da tensão no enrolamento primário (Vf)

![nome](/relatorio_eletronica_1/tensaovf.png)

#### Amplitude da tensão sobre o resistor (Vo)

![nome](/relatorio_eletronica_1/vo.png)

#### Amplitude da tensão no Vin e na tensão sobre o resistor (Vo)

![nome](/relatorio_eletronica_1/vinvo.png)

Para que o diodo seja polarizado necessita-se de uma tensão mínima (nesse caso de 0,72V), por isso podemos ver que no ramo de Vin até Vo intermediado por um diodo há uma queda de tensão de 0,7V o que consta no gráfico, onde Vin tem uma amplitude maior que Vo correspondente a queda de tensão que o diodo aplica sobre o circuito.

#### Tensão média eficaz de Vin

![nome](/relatorio_eletronica_1/vinvalor.png)

#### Tensão média eficaz de Vo

![nome](/relatorio_eletronica_1/vovalor.png)

#### Características do Diodo

![nome](/relatorio_eletronica_1/diodo11.png)

O valor medio de corrente que passa pelo diodo é de 18,74mA, a corrente máxima é de aproximadamente 60,12mA e o valor eficaz de corrente é de 29,76mA.

#### Circuito retificador de meia onda com capacitor de 330μF.

![nome](/relatorio_eletronica_1/capacitor.png)

#### Amplitude de onda da tensão (Vin) e da tensão sobre o resistor (Vo)

![nome](/relatorio_eletronica_1/capacitorvinvo.png)

A adição do capacitor no circuito tem um objetivo muito simples, diminuir a taxa de variação da tensão de saída sobre o resistor. Durante o ciclo positivo da tensão alternada do circuito o capacitor é carregado, e durante o ciclo negativo é descarregado, porém, como não é instantâneo a perda de tensão em cima do capacitor isso faz com que a tensão em cima do resistor não seja instantaneamente zero.

#### Valores de tensão média e eficaz sobre o resistor.

![nome](/relatorio_eletronica_1/vocapaci.png)

#### Formato de onda da corrente sobre o diodo.

![nome](/relatorio_eletronica_1/diodocapaci.png)

 O valor médio foi de 147,28mA e o valor eficaz 435,89mA e o valor máximo da corrente foi de aproximadamente 2,08A.

#### Circuito retificador de meia onda com capacitor de 2200μF

![nome](/relatorio_eletronica_1/capacitor2200.png)

#### Amplitude de onda da tensão (Vin) e da tensão sobre o resistor (Vo)

![nome](/relatorio_eletronica_1/vinvocapac.png)

Com o aumento do capacitor podemos perceber que há uma diminuição na tensão de ondulação do circuito (ripple) diminuindo a variação de tensão do circuito.

#### Valores de tensão média e eficaz sobre o resistor.

![nome](/relatorio_eletronica_1/vovalue.png)

#### Formato de onda da corrente sobre o diodo.

![nome](/relatorio_eletronica_1/d1value.png)

 O valor médio foi de 751,66mA e o valor eficaz 2,74A e o valor máximo da corrente foi de aproximadamente 13,65A.
