# Roteiro Final

## Parte 01

##### PROCEDIMENTO:

Considerando o circuito da figura 01 que representa uma fonte linear com regulador MOSFET, temos o seguinte problema:
1. Qual relação entre a tensão de alimentação do ampop e a tensão de saída?
2. O que devemos considerar para esse circuito operar como um LDO?
3. Como obter as tensões de alimentação para o AmpOp (VCC e VEE)?

Circuito proposto (01) para a alimentação do AmpOp:
4. Utilizando o circuito dobrador de tensão, qual valor de VCC você obtêm para um sinal Vin+ de 12Vrms?
5. Quais problemas apresentam esse circuito?
6. Podemos melhorar?

Circuito proposto (02) para a alimentação do AmpOp:
7. Vamos projetar esse circuito?

Considere:
- AmpOp LM324;
- MOSFET IRF540;
- VOUT = 15V;
- IOUT = 1A;
- Vin+ = 12Vrms;
- Vripple_pós_retificador = 1V;
- Quedas de tensão nos diodos = 0,7V.

### CIRCUITO DA FIGURA 01

Fonte linear com regulador MOSFET

![figura01](/resources/imagens/relatoriofinal/parte1/figura01.png)

#### RELAÇÃO ENTRE A TENSÃO DE ALIMENTAÇÃO DO AMPOP E A TENSÃO DE SAÍDA

Analisando o circuito da figura 1, podemos afirmar que a tensão de saída do circuito está limitada aos valores de alimentação do AmpOp, ou seja, na saída não teremos valores superiores a +Vcc ou inferiores a –Vcc os quais correspondem à saturação do AmpOp.

#### CONSIDERAÇÕES PARA O CIRCUITO OPERAR COMO UM LDO

Para o circuito operar como um regulador de baixa tensão (LDO), a tensão de entrada deve ser sempre superior à sua tensão de regulagem nominal, e a queda de tensão na saída deverá ser baixa. Temos que, a tensão de saída necessita da tensão de referência zener e da relação do R2 e R3, como apresentado na formula: Vout = Vz.(1+(R2/R3)).

#### TENSÃO DE ALIMENTAÇÃO PARA O AMPOP (VCC e VEE)

Para obter os valores de alimentação do ampop, devemos analisar os dados presentes no datasheet do ampop LM324. Iremos utilizar um dobrador de tensão para alimentar o VCC.

![datasheetlm324](/resources/imagens/relatoriofinal/parte1/datasheetlm324.png)

### CIRCUITO PROPOSTO (01) PARA A ALIMENTAÇÃO DO AMPOP

![circuitoproposto01](/resources/imagens/relatoriofinal/parte1/circuitoproposto01.png)

#### VALOR DE VCC - PROBLEMAS - SOLUÇÕES

Para o valor de VCC terá uma tensão de aproximadamente 33,55 V, o problema é que com a adição de uma carga na saída do terminal VCC a tensão de ripple irá aumentar. Como solução para diminuição da tensão de ripple, será colocado em serie após o circuito dobrador de tensão um circuito regulador do tipo série. Como apresentado no circuito proposto 02.

#### CIRCUITO DOBRADOR DE TENSÃO

Para alimentação do AmpOp com o circuito dobrador de tensão vamos considerar os dados já calculados anteriormente no roteiro 3 parte 1. Lembrando que a corrente de alimentação será considerada sendo ela 0,1A e a tensão de ripple em 10%. Logo, temos que:

C = I / Vr.f
C = 0,1 / 3,3.60
C = 505,05 uF

![circuitodobradortensao](/resources/imagens/relatoriofinal/parte1/circuitodobradortensao.png)

##### Onda da tensão de saída do circuito dobrador

![ondadobradortensao](/resources/imagens/relatoriofinal/parte1/ondadobradortensao.png)

Como apresentado anteriormente no datasheet do AmpOp LM324, do fabricante Texas Instruments, a faixa de fonte de alimentação singular do AmpOp deve ser de 3V a 32V. Será utilizado um diodo zener como referencia de tensão de alimentação, pelo fato da tensão de saída do circuito dobrador ser maior que 32V.

#### CIRCUITO REGULADOR DO DOBRADOR

Agora iremos adicionar o diodo zener, sabendo que como o AmpOp LM324 informado pelo seu datasheet anteriormente nos diz que a alimentação singular é de 3V a 32V, selecionamos o diodo zener UMZ27K da fabricante ROHM Semiconductor e o transistor 2N3904 da NXP, por possuir um hfe elevado. Com o intuito de diminuir a oscilação da tensão de saída do circuito dobrador.

![circuitoreguladordobrador](/resources/imagens/relatoriofinal/parte1/.png)

A tensão de saída calculada é de Vcc = Vz - VBR = 26,3V.

##### Onda da tensão de saída do circuito regulador do dobrador

![ondadobradortensao](/resources/imagens/relatoriofinal/parte1/.png)

O Vcc apresentado foi de XV.

### CIRCUITO PROPOSTO (02) PARA A ALIMENTAÇÃO DO AMPOP

![circuitoproposto02](/resources/imagens/relatoriofinal/parte1/circuitoproposto02.png)

#### TRANSFORMADOR

O transformador ira operar transformando 220V em 12Vrms, possuindo a mesma frequência da rede elétrica de 60hz. Como observador no circuito proposto (02) o retificador utilizado é do tipo de onda completa com transformação em derivação. Na teoria, temos que a queda de tensão em cada diodo é de 0,7V e o valor da tensão de pico é de 17V, calculando temos que o valor de pico da tensão de saída do retificador é de aproximadamente 16,3V.

#### RETIFICADOR

Retificadores são circuitos que correspondem a conversão de corrente alternada em corrente continua.

![retificador](/resources/imagens/relatoriofinal/parte1/retificador.png)

Na saída do circuito foi dimensionado um resistor de 16,3Ω, com a corrente máxima de 1A para coincidir com o valor de pico da tensão de saída de 16,3V.

##### Onda da tensão do enrolamento primário (Vs)

![ondaprimario](/resources/imagens/relatoriofinal/parte1/ondaprimario.png)

##### Onda da tensão do enrolamento secundário (Vin+) e na saída do circuito (Vout)

![ondasecundario](/resources/imagens/relatoriofinal/parte1/ondasecundario.png)

Como se pode observar o valor obtido para a tensão de pico na saída do circuito (Vout) foi de 16,04V.

#### FILTRO

Para o primeiro bloco (D1, D2 e C1) considere:
- Vin+ = 12Vrms;
- Vripple_pós_retificador = 1V;
- I_carga = 1,1A.

Devemos realizar a filtragem da corrente continua, pois a mesma não está pura, sendo assim, não servindo para alimentar o circuito eletrônico. Iremos utilizar uma das maneiras mais simples de filtragem que será o filtro tipo capacitivo.

Usaremos 1,1A para o circuito, sendo a limitação do AmpOp de 10mA, também usaremos 60hz para frequência e 1V para tensão de ripple.

Vrpp = Vout/2.R.f.C = I/2.f.C
C = I/(2.f.Vrrp)
C = 1,1/(2.60.1)
C =  9,1667mF

![circuitofiltro](/resources/imagens/relatoriofinal/parte1/circuitofiltro.png)

![ondafiltro](/resources/imagens/relatoriofinal/parte1/ondafiltro.png)

Como podemos conferir que o valor de Vrpp foi de aproximadamente 0,72V.

#### PROJETANDO O CIRCUITO PROPOSTO (02)

Utilizando as considerações apresentadas anteriormente:
- AmpOp LM324;
- MOSFET IRF540;
- VOUT = 15V;
- IOUT = 1A;
- Vin+ = 12Vrms;
- Vripple_pós_retificador = 1V;
- Quedas de tensão nos diodos = 0,7V.

![projcircuitoproposto02](/resources/imagens/relatoriofinal/parte1/.png)

![ondaprojcircuitoproposto02](/resources/imagens/relatoriofinal/parte1/.png)

xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
