# Roteiro Final

## Parte 02: Calculando e dimensionando os componentes

##### PROCEDIMENTO:

Circuito referência de tensão zener (R1 e D3): Ver roteiro 03.
1. Podemos melhorar esse circuito? Quais problemas podemos identificar nesta topologia?

Sugestão de melhoria:
2. No qual o circuito com R1, R5, Q2 e Q3 é uma fonte de corrente constante para polarizar o diodo zener D3. Vamos projetar?
3. Podemos melhorar mais ainda? Que tal deixar essa fonte com valor ajustável? Como fazer isso?
4. Escolhendo o transistor M1 e calculando R2 e R3.

### CIRCUITO REFERÊNCIA DE TENSÃO ZENER

![circuitoreferencia](/resources/imagens/relatoriofinal/parte2/circuitoreferencia.png)

Se a tensão sobre o resistor R1 for maior que 7V, o diodo zener não ficará polarizado e o regulador de tensão não terá mais a tensão de referência. Para melhorar o sistema se utilizará dois transistores PNP com o proposito de construir uma fonte de corrente que permita que o diodo zener não fique dependente da corrente que passa sobre o resistor R1 para ser polarizado.

### SUGESTÃO DE MELHORA

![sumelhora](/resources/imagens/relatoriofinal/parte2/sumelhora.png)

![sumelhora2](/resources/imagens/relatoriofinal/parte2/sumelhora2.png)

Para dimensionamento dos componentes:

![dimensionamento](/resources/imagens/relatoriofinal/parte2/dimensionamento.png)

### PROJETANDO O CIRCUITO PROPOSTO

![projcircuito](/resources/imagens/relatoriofinal/parte2/projcircuito.png)

Dados dos componentes utilizados:
- transistor PNP 2N3906 do fabricante NXP
- valor adotado para R5 foi de 25kΩ

#### Onda da tensão de saída Vout com carga de 15Ω

![vout15](/resources/imagens/relatoriofinal/parte2/vout15.png)

![vout151](/resources/imagens/relatoriofinal/parte2/vout151.png)

- Tensão de saída foi de 14,98V.
- Tensão de ripple foi de 509.26uV.

#### Onda da tensão e corrente sobre o diodo zener D3, com carga na saída de 15Ω

![tensaocorrentezener](/resources/imagens/relatoriofinal/parte2/tensaocorrentezener.png)

- Tensão sobre o diodo zener foi de 9,98V.
- Corrente sobre o diodo zener ficou entre 2,24mA e 2,34mA.

### Podemos melhorar mais ainda? Que tal deixar essa fonte com valor ajustável? Como fazer isso?

Uma melhora para deixar a fonte com valor ajustável seria a aplicação de um potenciômetro ligado em paralelo com o diodo zener (D3), assim possibilitando a mudança do valor de tensão de saída.
