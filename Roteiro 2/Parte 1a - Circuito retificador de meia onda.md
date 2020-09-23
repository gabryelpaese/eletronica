# Roteiro 2

## Parte 01_a: Circuito Retificador de Meia Onda

##### PROCEDIMENTO:

1. Simule o circuito do retificador de meia onda mostrado na Figura 1, inicialmente sem capacitor, anotando os valores na Tabela 1.
2. Em seguida adicione um capacitor eletrolítico de 330 µF na saída do retificador, conforme mostrado na Figura 2. Anote os valores solicitados na Tabela 1.
3. Substitua o capacitor eletrolítico de 330 µF por um de 2200 µF e observe a forma da tensão de saída do circuito, meça as grandezas solicitadas e anote na Tabela 1.
4. Verifique máxima tensão reversa nos diodos em cada um dos casos. Qual a corrente sobre o diodo?

Utilize L1 = 336,11uH e L2 = 1uH diretiva do spice “k L1 L2 1”

### CIRCUITO RETIFICADOR DE MEIA ONDA SEM CAPACITOR

![circuitosemcapacitor](/resources/imagens/relatorio2/parte1a/circuitosemcapacitor.png)

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO PRIMÁRIO (Vf)

![ondatensaoprimario](/resources/imagens/relatorio2/parte1a/ondatensaoprimario.png)

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO SECUNDÁRIO (Vin) E DA TENSÃO SOBRE O RESISTOR (Vo)

![ondatensaosecundario](/resources/imagens/relatorio2/parte1a/ondatensaosecundario.png)
![ondatensaosecundario2](/resources/imagens/relatorio2/parte1a/ondatensaosecundario2.png)

A onda Vout tem amplitude menor que a onda Vin, por causa da queda de tensão de 7,6V sobre o diodo para que o mesmo seja diretamente polarizado. O sinal de tensão Vout é zero no ciclo negativo de Vin por causa da polarização inversa do diodo.

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO SECUNDÁRIO (Vin) E DA TENSÃO SOBRE O RESISTOR (Vo)

![tensaomedia](/resources/imagens/relatorio2/parte1a/tensaomedia.png)
![tensaomedia2](/resources/imagens/relatorio2/parte1a/tensaomedia2.png)

#### TABELA DOS VALORES MEDIDOS SEM CAPACITOR

![tabelasemcapacitor](/resources/imagens/relatorio2/parte1a/tabelasemcapacitor.png)

#### ONDA DA CORRENTE SOBRE O DIODO (D1)

![ondacorrentediodo](/resources/imagens/relatorio2/parte1a/ondacorrentediodo.png)

Valor máximo da corrente = 60 mA

Valor médio da corrente = 18,62 mA

Valor eficaz da corrente = 29,61 mA

### CIRCUITO RETIFICADOR DE MEIA ONDA COM CAPACITOR DE 330μF

![circuito330](/resources/imagens/relatorio2/parte1a/circuito330.png)

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO SECUNDÁRIO (Vin) E DA TENSÃO SOBRE O RESISTOR (Vo)

![ondatensao](/resources/imagens/relatorio2/parte1a/ondatensao.png)
![ondatensao2](/resources/imagens/relatorio2/parte1a/ondatensao2.png)

Com a presença do capacitor o circuito tem um redução na sua taxa de variação de tensão Vo sobre o resistor. Em Vin no ciclo positivo o capacitor é carregado, e no ciclo negativo o capacitor vai sendo descarregado ao longo do tempo, com isso a tensão sobre o resistor não será zero. A diferença entre a tensão máxima de Vo e a tensão de Vo quando o capacitor começa a carregar novamente é a tensão de ripple. Nesse caso a tensão de ripple é de 1,73V.

#### VALORES DE TENSÃO MÉDIA E EFICAZ SOBRE O RESISTOR (Vo)

![tensaomedia3](/resources/imagens/relatorio2/parte1a/tensaomedia3.png)

#### TABELA DOS VALORES MEDIDOS

![tabelasemcapacitor2](/resources/imagens/relatorio2/parte1a/tabelasemcapacitor2.png)

#### FORMATO DE ONDA DA CORRENTE SOBRE O DIODO (D1)

![ondacorrentediodo2](/resources/imagens/relatorio2/parte1a/ondacorrentediodo2.png)
![extra](/resources/imagens/relatorio2/parte1a/extra.png)

Valor máximo da corrente = 2,10 A

Valor médio da corrente = 101,19 mA

Valor eficaz da corrente = 350,45 mA

### CIRCUITO RETIFICADOR DE MEIA ONDA COM CAPACITOR DE 2200μF

![circuito2200](/resources/imagens/relatorio2/parte1a/circuito2200.png)

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO SECUNDÁRIO (Vin) E DA TENSÃO SOBRE O RESISTOR (Vo)

![ondatensao3](/resources/imagens/relatorio2/parte1a/ondatensao3.png)
![ondatensao4](/resources/imagens/relatorio2/parte1a/ondatensao4.png)

Com o aumento da capacitância do circuito o valor da tensão de ripple diminuiu, indo para 0,29V.

#### VALORES DE TENSÃO MÉDIA E EFICAZ SOBRE O RESISTOR (Vo)

![tensaomedia4](/resources/imagens/relatorio2/parte1a/tensaomedia4.png)

#### TABELA DOS VALORES MEDIDOS

![tabelasemcapacitor3](/resources/imagens/relatorio2/parte1a/tabelasemcapacitor3.png)

#### FORMATO DE ONDA DA CORRENTE SOBRE O DIODO (D1)

![ondacorrentediodo3](/resources/imagens/relatorio2/parte1a/ondacorrentediodo3.png)

Valor máximo da corrente = 14,03 A

Valor médio da corrente = 406,28 mA

Valor eficaz da corrente = 1,985 A

### RESULTADOS

Tensões sobre os resistores

![resultado1](/resources/imagens/relatorio2/parte1a/resultado1.png)

Concluiu-se que ao conectar capacitores em paralelo é possível mandar sobre o resistor um valor de tensão próximo a tensão de pico do enrolamento secundário, porem para diminuir a tensão de ripple é necessários que o valor da capacitância aumente.

Formas de onda da corrente sobre os diodos

![resultado2](/resources/imagens/relatorio2/parte1a/resultado2.png)

Toda vez que o capacitor carrega existe um pico de corrente (sendo maior na primeira vez que é carregado) que aumenta dependendo do valor da capacitância do capacitor.
