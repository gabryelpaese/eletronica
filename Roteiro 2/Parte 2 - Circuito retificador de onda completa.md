# Roteiro 2

## Parte 02: Circuito Retificador de Onda Completa

##### PROCEDIMENTO:

1. Monte o circuito retificador de onda completa em ponte usando transformador, conforme mostrado nas Figuras 3 e 4. Anote os valores solicitados na Tabela 1.

### CIRCUITO RETIFICADOR DE MEIA ONDA SEM CAPACITOR

![circuitosemcapacitor]()

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO PRIMÁRIO (Vf)

![ondatensaoprimario]()

#### FORMATO DE ONDA DA TENSÃO NO ENROLAMENTO SECUNDÁRIO (Vin) E DA TENSÃO SOBRE O RESISTOR (Vo)

![ondatensaosecundario]()
![ondatensaosecundario2]()

É possível perceber que a onda Vo tem amplitude um pouco menor do que a onda Vin. Isso acontece por conta da queda de tensão de 7,6V sobre o diodo para que o mesmo seja polarizado diretamente. O valor do sinal de tensão Vo é zero nos ciclos negativos de Vin por conta da polarização inversa do diodo.

#### Valores de tensão média e eficaz sobre o enrolamento secundário (Vin) e o resistor (Vo)

![]()
![]()

#### Tabela dos valores medidos sem CAPACITOR

![]()

#### Onda da corrente sobre o diodo (D1)

![]()
![]()

O valor máximo da corrente foi de 41,65mA, o valor médio foi de 12,81mA e o valor eficaz foi de 28,48mA.

### Circuito retificador de meia onda com capacitor de 330μF

O diodo utilizado nas simulações foi o disponibilizado pelo próprio LTspice.
![]()

#### Formato de onda da tensão no enrolamento secundário (Vin) e da tensão sobre o resistor (Vo)

![]()
![]()

A adição do capacitor no circuito faz com que a taxa de variação da tensão Vo sobre o resistor diminua consideravelmente.

No ciclo positivo de Vin o capacitor é carregado, e então no seu ciclo negativo o capacitor vai descarregando fazendo com que a tensão sobre o resistor não seja zero (como foi visto no circuito anterior). Quando Vin entrar no ciclo positivo o capacitor vai começar a carregar novamente.

A diferença entre a tensão máxima de Vo e a tensão de Vo quando o capacitor começa a carregar novamente é a tensão de ripple. Nesse caso a tensão de ripple é de 1,73V.

#### Valores de tensão média e eficaz sobre o resistor (Vo)

![]()

#### Preenchimento da tabela com os valores solicitados

![]()

#### Formato de onda da corrente sobre o diodo (D1)

![]()
![]()

O valor máximo da corrente foi de 1,48A, o valor médio foi de 102,06mA e o valor eficaz foi de 317,72mA.

### Simulação: Circuito retificador de meia onda com capacitor de 2200μF

![]()

#### Formato de onda da tensão no enrolamento secundário (Vin) e da tensão sobre o resistor (Vo)

![]()
![]()

Com o aumento da capacitância do capacitor do circuito o valor da tensão de ripple diminuiu, sendo de 0,29V.

#### Valores de tensão média e eficaz sobre o resistor (Vo)

![]()

#### Preenchimento da tabela com os valores solicitados

![]()

#### Formato de onda da corrente sobre o diodo (D1)

![]()
![]()

O valor máximo da corrente foi de 9,90A, o valor médio foi de 522,57mA e o valor eficaz foi de 1,98A.
