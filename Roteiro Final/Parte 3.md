# Roteiro Final

## Parte 03: Adicionando um circuito de proteção de sobre corrente ao regulador linear

##### PROCEDIMENTO:

1. Primeiramente reflita e pesquise sobre o que é sobrecorrente?
2. Quais os impactos neste circuito?
3. O que deve fazer um circuito de proteção de sobrecorrente?
4. O que é a proteção foldback?
5. Pesquise as topologias disponíveis, caso deseja-se fazer um circuito LDO, o que devemos levar em consideração para o regulador?

#### O que é sobrecorrente?

É quando uma corrente cujo o valor excede o valor suportável pelo condutor.

#### Quais os impactos neste circuito?

Com a ocorrência de sobrecorrente no circuito, acarretará a danificar e comprometer a vida útil de componentes eletrônicos, podendo queima-los.

#### O que deve fazer um circuito de proteção de sobrecorrente? O que é a proteção foldback?

O circuito de proteção de sobrecorrente irá agir desviando parte da corrente quando atingir um valor maior que o previsto para que não ocorra a sobrecorrente queimando os componentes.

Outra maneira do circuito de proteção de sobrecorrente é o sistema de proteção foldback que irá agir diminuindo a tensão sobre o condutor e consequentemente a corrente ira diminuir também,  diminuindo a tensão de saída e da corrente sobre a carga.

### Para um circuito LDO, o que devemos levar em consideração para o regulador?

#### SUGESTÃO DE MELHORA

![circuitoproposto](/resources/imagens/relatoriofinal/parte3/circuitoproposto.png)

Dados dos componentes utilizados:
- transistor NMOS 2N7002 do fabricante DIODES Semiconductor
- Resistencia shunt = 30mΩ
- VDS = Vt = 2,154V

##### Cálculo de R7 e R9

![calculor7r9](/resources/imagens/relatoriofinal/parte3/calculor7r9.png)

### PROJETANDO O CIRCUITO PROPOSTO

![projcircuito](/resources/imagens/relatoriofinal/parte3/projcircuito.png)

#### Tensão de saída sem carga

![saidasemcarga](/resources/imagens/relatoriofinal/parte3/saidasemcarga.png)

#### Tensão e corrente com carga de 15Ω

![saidacarga15](/resources/imagens/relatoriofinal/parte3/saidacarga15.png)

#### Tensão e corrente com carga de 3Ω

![saidacarga3](/resources/imagens/relatoriofinal/parte3/saidacarga3.png)
