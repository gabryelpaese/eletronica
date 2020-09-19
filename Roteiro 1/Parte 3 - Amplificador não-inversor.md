# Roteiro 1

## Parte 3: Amplificador não-inversor

##### OBJETIVOS:

Medir o ganho de um amplificador não-inversor.

##### EXPERIMENTO:

Utilizando um Amp.OP. Lm324N e o TL082 monte dois amplificadores não inversores use o resistor de realimentação com valor 20 kΩ e o outro resistor igual à 2kΩ. Utilize a alimentação simétrica de +/-12V. (limite a corrente em 0,05A)

##### PROCEDIMENTO:

1. Monte o circuito em uma matriz de contatos (protoboard) e antes de ligar as fontes chame
o professor.
2. Configure no gerador de função um sinal senoidal com 0,5Vp @ 1 kHz e mostre o mesmo
no canal 1 do osciloscópio.
3. Mostre a saída do amplificador no canal 2 do osciloscópio e chame o professor novamente
e mostre os resultados.
4. Verifique o valor do ganho obtido;
5. Qual o valor da queda de tensão com relação a tensão de alimentação?

### CALCULO PARA O GANHO DE TENSÃO (AV):

![calculoganhodetensao](/resources/imagens/relatorio1/parte3/calculoganhodetensao.jpeg)

### DE ACORDO COM O CIRCUITO AMPLIFICADOR NÃO-INVERSOR O FORMATO DE ONDA DA TENSÃO DE ENTRADA:

![ondatensaoentrada](/resources/imagens/relatorio1/parte3/ondatensaoentrada.png)
![cursorentrada](/resources/imagens/relatorio1/parte3/cursorentrada.png)

### CIRCUITO AMPLIFICADOR NÃO-INVERSOR COM O AMPOP LM324M

![circuitoinversorlm324m](/resources/imagens/relatorio1/parte3/circuitoinversorlm324m.png)

Tensão de saída do circuito:

![tensaosaidalm324m](/resources/imagens/relatorio1/parte3/tensaosaidalm324m.png)
![cursorsaidalm324m](/resources/imagens/relatorio1/parte3/cursorsaidalm324m.png)

Comparação entre tensão de entrada e saída do circuito:

![comparacaosaidaentradalm324m](/resources/imagens/relatorio1/parte3/comparacaosaidaentradalm324m.png)

### CIRCUITO AMPLIFICADOR NÃO-INVERSOR COM O AMPOP TL082

![circuitoinversortl082](/resources/imagens/relatorio1/parte3/circuitoinversortl082.png)

Tensão de saída do circuito:

![tensaosaidatl082](/resources/imagens/relatorio1/parte3/tensaosaidatl082.png)
![cursorsaidatl082](/resources/imagens/relatorio1/parte3/cursorsaidatl082.png)

Comparação entre tensão de entrada e saída do circuito:

![comparacaosaidaentradatl082](/resources/imagens/relatorio1/parte3/comparacaosaidaentradatl082.png)

### RESULTADOS SIMULAÇÕES

Nos dois circuitos simulados anteriormente a amplitude do sinal da tensão de saída é de 5,51V e 5,48V, correspondendo a um ganho de 11 vezes o valor de entrada.

### ANÁLISE DE SATURAÇÃO: CIRCUITO COM LM324N

Sinal de tensão de saída do circuito com 0,99V de amplitude na tensão de entrada (saturação positiva):

![saturacaolm324m](/resources/imagens/relatorio1/parte3/saturacaolm324m.png)
![2saturacaolm324m](/resources/imagens/relatorio1/parte3/2saturacaolm324m.png)
![cursorsaturacaolm324m1](/resources/imagens/relatorio1/parte3/cursorsaturacaolm324m1.png)

Na tensão 10,77V ocorreu saturação positiva tendo um valor de queda de tensão de 1,23V.


Sinal de tensão de saída do circuito com 1,04V de amplitude na tensão de entrada (saturação negativa e positiva):

![3saturacaolm324m](/resources/imagens/relatorio1/parte3/3saturacaolm324m.png)
![4saturacaolm324m](/resources/imagens/relatorio1/parte3/4saturacaolm324m.png)
![cursorsaturacaolm324m2](/resources/imagens/relatorio1/parte3/cursorsaturacaolm324m2.png)
![5saturacaolm324m](/resources/imagens/relatorio1/parte3/5saturacaolm324m.png)
![cursorsaturacaolm324m3](/resources/imagens/relatorio1/parte3/cursorsaturacaolm324m3.png)

Na tensão -11,33V ocorreu saturação negativa, tendo um valor de queda de tensão de -0,67V. Saturação positiva continua sendo 10,77V.

### ANÁLISE DE SATURAÇÃO: CIRCUITO COM TL082

Sinal de tensão de saída do circuito com 1,40V de amplitude na tensão de entrada (saturação positiva e negativa):

![saturacaotl082](/resources/imagens/relatorio1/parte3/saturacaotl082.png)
![2saturacaotl082](/resources/imagens/relatorio1/parte3/2saturacaotl082.png)
![cursorsaturacaotl082](/resources/imagens/relatorio1/parte3/cursorsaturacaotl082.png)
![3saturacaotl082](/resources/imagens/relatorio1/parte3/3saturacaotl082.png)
![cursorsaturacaotl0822](/resources/imagens/relatorio1/parte3/cursorsaturacaotl0822.png)

Na tensão 10,47V ocorreu saturação positiva e na tensão de -10,47 ocorreu a saturação negativa, tendo um valor de queda de tensão de 1,53V e -1,53V.

### RESULTADOS SATURAÇÃO

Foi observado que o sinal é amplificado e não invertido utilizando o circuito do AmpOp Não Inversor. Nesse experimento o sinal de saída tinha a amplitude onze vezes maior do que o sinal de entrada e os ciclos positivos e negativos do sinal de saída coincidiam com os do sinal de entrada.

Como foi esperado para essa simulação o sinal de tensão de saída dependente da tensão de alimentação que nesse caso foi de 12V. Testando os AmpOp LM324M observamos que o mesmo apresenta tensões de saturação diferentes (10,77V e -11,33V) e o AmpOp TL082 as tensões de saturação foram as mesmas (+-10,47). Isso mostra que as especificações técnicas entre esses dois elementos são diferentes, possuindo diferenças na zona de saturação.
