# Roteiro 4

## Parte 04 - Inversor com transistor do tipo NMOS (NMOS Inverter):

#### Objetivo:

1. Simular o circuito abaixo

![nome](/relatorio_eletronica_1/figura04.png)

 R1 = 10 kΩ

 VCC= 5,0 V.

 VIN = forma de onda quadrada com frequência de 1 kHz

 Amplitude= 5,0 Vpp (sem valor negativo, ou seja de 0 a 5V).

2. Comparar as formas de onda de entrada e de saída.

3. Obter o valor de RDS para esse transistor para esta condição de operação.

4. Caso sinal de entrada tenha(VIN) a amplitude reduzida para 2,5 V, achar o valor de RDS

5. Comparar os resultados obtidos na simulação com a teoria.

### Circuito Simulado

![nome](/relatorio_eletronica_1/circsim1.png)

#### Utilizando Vin 5V

#### Forma de onda de entrada

![nome](/relatorio_eletronica_1/vinvin1.png)


#### Forma de onda de saída

![nome](/relatorio_eletronica_1/voutout1.png)

![nome](/relatorio_eletronica_1/draft.png)


#### Utilizando Vin 2.5V

#### Forma de onda de entrada

![nome](/relatorio_eletronica_1/vin255.png)


#### Forma de onda de saída

![nome](/relatorio_eletronica_1/vo255.png)

![nome](/relatorio_eletronica_1/vo25.png)

#### Valor de RDS para a condição específica

![nome](/relatorio_eletronica_1/vin05.png)

Utilizando Vin = 5V obtive um RDS de 0,76 Ohms e uma tensão de saída Vout = 379µV

#### Valor de RDS caso Vin seja reduzido para 2.5V


![nome](/relatorio_eletronica_1/vin25.png)

Quando mudamos a tensão de entrada para 2.5V percebe-se que houve um aumento significativo em RDS de 0,76 Ohms para 6,28 Ohms, com isso, o cálculo da tensão de saída também houve mudança significativa passando de 379µV para 1,56mV.

#### Comparação dos resultados obtidos na simulação com a teoria

##### Utilizando Vin 5V:

Teórico: Vout = 379µV

Simulado: Vout = 865µV

Quando comparamos a porcentagem correspondente do resultado teórico com o simulado, obtemos um valor correspondente a 43,81% em relação ao Vout simulado.

##### Utilizando Vin 2,5V:

Teórico: Vout = 1,56mV

Simulado: Vout = 3,61mV

Quando comparamos a porcentagem correspondente do resultado teórico com o simulado, obtemos um valor correspondente a 43,21% em relação ao Vout simulado.

Em ambos os casos o valor correspondente fica na casa dos 43% de diferença, motivo pelo qual eu não tenho informações ou conhecimento suficiente para obter conclusões precisas.
