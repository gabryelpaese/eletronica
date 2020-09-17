# Roteiro 1

## Parte 1: Seguidor de Tensão

##### OBJETIVOS:

Verificar o funcionamento de um circuito seguidor de tensão.

##### EXPERIMENTO:

Utilizando um Amp.OP. Lm324N e um TL082 monte dois circuitos na configuração de seguidor de tensão (Buffer), com uma resistência de realimentação de 10 kΩ em cada um dos circuitos. Utilize a alimentação simétrica de +/-12V (limite a corrente em 0,05A).

##### PROCEDIMENTO:

1. Monte o circuito em uma matriz de contatos (protoboard) e antes de ligar as fontes chame o professor.
2. Configure no gerador de função um sinal senoidal com 0,5Vp @ 1 kHz e mostre o mesmo no canal 1 do osciloscópio.
3. Discuta os resultados.


### CALCULO PARA O GANHO DE TENSÃO (AV):
![p1conta1]()

### DE ACORDO COM O CIRCUITO SEGUIDOR DE TENSÃO O FORMATO DE ONDA DA TENSÃO DE ENTRADA:
![tensaofonte]()

### CIRCUITO SEGUIDOR DE TENSÃO COM O AMPOP LM324M
![Circuito1p1]()

Tensão de saída do circuito:
![p1onda1]()

Comparação entre tensão de entrada e saída do circuito:
![p1onda1]()

### CIRCUITO SEGUIDOR DE TENSÃO COM O AMPOP TL082
![Circuito2p1]()

Tensão de saída do circuito:
![p1onda2]()

Comparação entre tensão de entrada e saída do circuito:
![p1onda2]()

### RESULTADOS
O seguidor de tensão, fornece um ganho unitário sem inversão de polaridade ou fase. Portanto a saída possui mesma amplitude, polaridade e fase de entrada. O circuito atua como isolador (buffer) de estágios, reforçador de correntes e casador de impedâncias.
Nos experimentos analisamos que a tensão RMS de entrada é aproximadamente igual a tensão RMS de saída nos AmpOp TL082 e LM324M, tendo uma diferença insignificante.
