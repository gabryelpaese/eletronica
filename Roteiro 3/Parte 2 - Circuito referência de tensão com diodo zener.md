# Roteiro 3

## Parte 02: Circuito referência de tensão com diodo Zener

##### PROCEDIMENTO:

1. Adicione a saída do dobrador de tensão do circuito anterior um regulador shunt para a referência de tensão.
Projete este circuito considerando:
2. A tensão zener dever ser igual á tensão miníma de saída menos 2V, ou seja, Vz = Vp -Vr -2V. Onde Vp é a tensão máxima na saída do dobrador e Vr é tensão de ripple.
3. Escolha o diodo zener de modo a minimizar o consumo neste circuito.
4. Qual a regulação de linha e qual a regulação de carga para este circuito?

### DATASHEET DO DIODO ZENER 1N4750A

![datasheet](/resources/imagens/relatorio3/parte2/datasheet.png)
![datasheet2](/resources/imagens/relatorio3/parte2/datasheet2.png)

### SITUAÇÃO 1:

#### CÁLCULO DA TENSÃO ZENER (Vz)

![calculozener](/resources/imagens/relatorio3/parte2/calculozener.png)

#### CIRCUITO REFERÊNCIA DE TENSÃO COM DIODO ZENER SITUAÇÃO 1

![circuitotensao](/resources/imagens/relatorio3/parte2/circuitotensao.png)

#### FORMATO DE ONDA SITUAÇÃO 1

![formatoonda](/resources/imagens/relatorio3/parte2/formatoonda.png)

### SITUAÇÃO 2:

#### CÁLCULO DA TENSÃO ZENER (Vz) COM IZ = 1,5mA

![calculozener2](/resources/imagens/relatorio3/parte2/calculozener2.png)

#### CIRCUITO REFERÊNCIA DE TENSÃO COM DIODO ZENER SITUAÇÃO 2

![circuitotensao2](/resources/imagens/relatorio3/parte2/circuitotensao2.png)

#### FORMATO DE ONDA SITUAÇÃO 2

![formatoonda2](/resources/imagens/relatorio3/parte2/formatoonda2.png)

### SITUAÇÃO 3:

#### CÁLCULO REGULAÇÃO DE LINHA E DE CARGA COM DIODO ZENER 1N4750A

![calculozener3](/resources/imagens/relatorio3/parte2/calculozener3.png)

#### CIRCUITO REFERÊNCIA DE TENSÃO COM DIODO ZENER SITUAÇÃO 3

![circuitotensao3](/resources/imagens/relatorio3/parte2/circuitotensao3.png)

#### FORMATO DE ONDA SITUAÇÃO 3

![formatoonda3](/resources/imagens/relatorio3/parte2/formatoonda3.png)

### RESULTADOS

#### SITUAÇÃO 1
Diferença na tensão de pico 30,90V, e a tensão Vcc 26,91V diferente do valor calculado.

#### SITUAÇÃO 2
Com a diminuição da corrente zener para 1,5mA, sofreram mudanças no resistor R e na tensão Vz0, resultando com a tensão de saída Vcc idêntica ao valor calculado.

#### SITUAÇÃO 3
