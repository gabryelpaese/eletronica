# Roteiro 4

## Parte 03: Espelho de corrente com transistores do tipo NMOS

##### PROCEDIMENTO:

1. Simule o circuito da Figura 02, com os seguintes valores: R1 = 1,0 kΩ, VCC= 10,0 V. Para R2, variando entre 0 e 100kΩ.
2. Explique o funcionamento deste circuito comparando as corrente ID1 e ID2.
3. Variando a resistência R2, trace a curva ID2 x V2.
4. Obtenha o máximo valor de R2 para o espelho de corrente funcionar corretamente.
5. Compare os resultados obtidos com a teoria.

### FUNCIONAMENTO DO CIRCUITO ESPELHO DE CORRENTE COM TRANSISTORES DO TIPO NMOS

O transistor Q1 está funcionando como um diodo, pois seus polos estão curto-circuitados, logo a corrente que passa por Q1 é a mesma que passa pelo R1, conhecida como Iref, esta corrente gera uma tensão VGS que polariza o transistor Q2, desta forma a corrente I2 será a mesma que passa por Q1. Por essa característica o circuito é denominado de espelho de corrente, onde Q1 é um conversor de corrente para tensão e Q2 conversor de tensão para corrente, concluindo que ID1 = ID2.

### CURVA IDS2 X V2 (VARIANDO R2)

#### CIRCUITO PARA ESPELHO DE CORRENTE COM TRANSISTORES NMOS

![circuitocurvaids2xv22](/resources/imagens/relatorio4/parte3/circuitocurvaids2xv22.png)

#### CURVA IDS2 X V2

![curvaids2xv2](/resources/imagens/relatorio4/parte3/.png)

### MÁXIMO VALOR DE R2 PARA O FUNCIONAMENTO DO ESPELHO DE CORRENTE

#### VALOR CALCULADO

![maxvalorr](/resources/imagens/relatorio4/parte3/maxvalorr.png)

#### CURVA IDS2 X R2

![curvaids2xr2](/resources/imagens/relatorio4/parte3/curvaids2xr2.png)
![curvaids2xr22](/resources/imagens/relatorio4/parte3/curvaids2xr22.png)

### COMPARAÇÃO DOS VALORES

![comparacaovaloress](/resources/imagens/relatorio4/parte3/comparacaovaloress.png)
![comparacaovalores22](/resources/imagens/relatorio4/parte3/comparacaovalores22.png)

### RESULTADOS
Para valores menores do que o valor máximo de R2 (1023,68 Ω), o transistor Q2 permanecerá tendo o valor mínimo de tensão Vt (2,154 V) para condução, ao contrario Q2 não estará em condução. A diferença entre o valor teórico e o calculado do R2 foi de 181,925 Ω.
