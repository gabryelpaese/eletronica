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

![calculoganhodetensao](/resources/imagens/relatorio1/parte1/calculoganhodetensao.jpeg)

### DE ACORDO COM O CIRCUITO SEGUIDOR DE TENSÃO O FORMATO DE ONDA DA TENSÃO DE ENTRADA:

![ondatensaoentrada](/resources/imagens/relatorio1/parte1/ondatensaoentrada.png)
![cursor](/resources/imagens/relatorio1/parte1/cursorentrada.png)

### CIRCUITO SEGUIDOR DE TENSÃO COM O AMPOP LM324M

![circuitolm324m](/resources/imagens/relatorio1/parte1/circuitolm324m.png)

Tensão de saída do circuito:

![tensaosaidalm324m](/resources/imagens/relatorio1/parte1/tensaosaidalm324m.png)
![cursorsaidalm324m](/resources/imagens/relatorio1/parte1/cursorsaidalm324m.png)

Comparação entre tensão de entrada e saída do circuito:

![comparaçaosaidaentradalm324m](/resources/imagens/relatorio1/parte1/comparaçaosaidaentradalm324m.png)
![2comparaçaosaidaentradalm324m](/resources/imagens/relatorio1/parte1/2comparaçaosaidaentradalm324m.png)

### CIRCUITO SEGUIDOR DE TENSÃO COM O AMPOP TL082

![](/resources/imagens/relatorio1/parte 1/)

Tensão de saída do circuito:

![](/resources/imagens/relatorio1/parte 1/)

Comparação entre tensão de entrada e saída do circuito:

![](/resources/imagens/relatorio1/parte 1/)
![](/resources/imagens/relatorio1/parte 1/)

### RESULTADOS
O seguidor de tensão, fornece um ganho unitário sem inversão de polaridade ou fase. Portanto a saída possui mesma amplitude, polaridade e fase de entrada. O circuito atua como isolador (buffer) de estágios, reforçador de correntes e casador de impedâncias.
Nos experimentos analisamos que a tensão RMS de entrada é aproximadamente igual a tensão RMS de saída nos AmpOp TL082 e LM324M, tendo uma diferença insignificante.
