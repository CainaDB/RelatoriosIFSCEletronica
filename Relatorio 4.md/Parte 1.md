# Relatório 4 -  Transistores do tipo MOS

## Parte 1: Parâmetros do transistor:

#### Objetivo:

Estudar as características e aplicações de circuitos com transistores do tipo MOS.

#### Procedimento:

1 - Simular os circuitos com os transistores do tipo NMOS.

2 - Analisar e discutir os resultados encontrados.

3 - Será utilizado para a simulação o transistor 2N7002 de dois fabricantes distintos (Nexperia e Diodes Incorporated).

### Parâmetros, Valores de RDS, Tensão máxima de operação e Curvas Id x Vds

![nome](/relatorio_eletronica_1/tabelammos.png)

O Cox foi calculado usando a fórmula Kp/Uo onde o Kp e o Uo foi retirado dos Datasheets e dos Models dos respectivos transistores.

![nome](/relatorio_eletronica_1/rds.png)

Os valores de RDS foram calculados utilizando a formula:
1/Kn*W/L(VGS - Vt).

Onde Kn é a transcondutância (Kp).

W/L são as dimensões.

VGS é a Tensão Ground Source (porta-fonte).

Vt é a tensão de limiar (threshold).


![nome](/relatorio_eletronica_1/diodesmaxi.png)

As tensões máximas de operação do transistor da Diodes Incorporated.

![nome](/relatorio_eletronica_1/nexperiamaxi.png)

As tensões máximas de operação do transistor da Nexperia.

### Curvas Id x VDS

Foi utilizado o transistor da Diode Incorporated para a análise gráfica.

![nome](/relatorio_eletronica_1/graficocorrente.png)

![nome](/relatorio_eletronica_1/comparativo.png)

Comparando o gráfico do simulado com o do datasheet do componente podemos notar uma diferença em relações aos fatores externos, por exemplo, no datasheet se leva em conta a temperatura enquanto no LTSpice isso é ignorado. Em geral, nos datasheets dos componentes há uma importância muito grande ao meio externo onde o componente é utilizado, todavia, em simulações de softwares é difícil trazer esse fator para dentro do programa e muitas vezes acaba prejudicando a simulação.

### Comparação com os valores teóricos

![nome](/relatorio_eletronica_1/tabelardss.png)
