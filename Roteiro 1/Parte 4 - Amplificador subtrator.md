# Roteiro 1

## Parte 4: Amplificador subtrator

##### OBJETIVOS:

Verificar as não idealidades dos ampops aplicadas em um circuito subtrator.

##### EXPERIMENTO:

Utilizando um Amp.OP. Lm324N e o TL082 monte dois amplificadores subtratores
use o resistor de realimentação com valor 510kΩ e ganho igual á 10V/V. Utilize a alimentação simétrica de +/-12V. (limite a corrente em 0,05A)

##### PROCEDIMENTO:

1. Monte o circuito em uma matriz de contatos (protoboard) e antes de ligar as fontes chame o professor.
2. Compare os resultados para o LM324N e para TL082.
3. Caso a fonte V1 tenha o valor igual á 0(zero)V, qual o valor da tensão de saída, para ambos os circuitos? Explique.
4. Caso o seja alterado para o circuito abaixo, existe alguma variação na saída? Explique.
5. Justifique as dissimilaridades encontradas utilizando os dados do datasheet.

### CALCULO DOS RESISTORES (R1):

![calculoresistores](/resources/imagens/relatorio1/parte4/calculoresistores.jpeg)


### CIRCUITO AMPLIFICADOR SUBTRATOR COM O AMPOP LM324M

![circuitoinversorlm324m](/resources/imagens/relatorio1/parte4/circuitoinversorlm324m.png)

### CIRCUITO AMPLIFICADOR SUBTRATOR COM O AMPOP TL082

![circuitoinversortl082](/resources/imagens/relatorio1/parte4/circuitoinversortl082.png)

### TENSÃO DE ENTRADA DE 12V COM APENAS UM RESISTOR DE 620Ω DE ENTRADA

Tensão de saída do circuito LM324N:

![tensaosaidalm324m](/resources/imagens/relatorio1/parte4/tensaosaidalm324m.png)

Tensão de saída do circuito TL082:

![tensaosaidatl082](/resources/imagens/relatorio1/parte4/tensaosaidatl082.png)

### TENSÃO DE ENTRADA DE 0V COM APENAS UM RESISTOR DE 620Ω DE ENTRADA

Tensão de saída do circuito LM324N:

![tensaosaidalm324m1](/resources/imagens/relatorio1/parte4/tensaosaidalm324m1.png)

Tensão de saída do circuito TL082:

![tensaosaidatl0822](/resources/imagens/relatorio1/parte4/tensaosaidatl0822.png)

### CIRCUITOS AMPLIFICADOR SUBTRATOR COM MAIS UM RESISTOR DE 620Ω DE ENTRADA

![circuitos](/resources/imagens/relatorio1/parte4/circuitos.png)

### TENSÃO DE ENTRADA DE 12V COM MAIS UM RESISTOR DE 620Ω DE ENTRADA

Tensão de saída do circuito LM324N:

![tensaosaidalm324m2](/resources/imagens/relatorio1/parte4/tensaosaidalm324m2.png)

Tensão de saída do circuito TL082:

![tensaosaidatl0823](/resources/imagens/relatorio1/parte4/tensaosaidatl0823.png)

### TENSÃO DE ENTRADA DE 0V COM MAIS UM RESISTOR DE 620Ω DE ENTRADA

Tensão de saída do circuito LM324N:

![tensaosaidalm324m3](/resources/imagens/relatorio1/parte4/tensaosaidalm324m3.png)

Tensão de saída do circuito TL082:

![tensaosaidatl0824](/resources/imagens/relatorio1/parte4/tensaosaidatl0824.png)

### COMPARAÇÃO SINAL DE SAIDA DOS CIRCUITOS COM AMPOP LM324M E TL082

Tensão de entrada de 12V:

![tensaoentrada12](/resources/imagens/relatorio1/parte4/tensaoentrada12.png)

Tensão de entrada de 0V:

![tensaoentrada0](/resources/imagens/relatorio1/parte4/tensaoentrada0.png)

### RESULTADOS SIMULAÇÕES
Comparando os dois circuitos simulados para a tensão de entrada de 12V, temos que com o AmpOp LM324N a tensão de saída é maior (128,12mV). Quando utilizado como tensão de entrada de 0V notasse que a tensão de saída do circuito LM32N fica menor (31,43mV) e a do circuito TL082 fica praticamente nula (120,67µV).
