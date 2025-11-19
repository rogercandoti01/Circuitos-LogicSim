# Circuitos-LogicSim
Yes
## 4-Bit-Adder
### Resumo
O circuito lógico é responsável por realizar a soma binária de dois números de 4 bits. Possui 1 half-adder, e 3 full-adder, onde o half faz os primeiros calculos e em sequencia os full-adder continuam utilizando os carrys dos calculos passados.
### Entradas
- A e B: Uma entrada 4-bit que dara o valor positivo para soma.
### Saidas
- Sum: Valor que resulta a soma de A e B.

## 4-Bit-Adder-Scale
### Resumo
O circuito logico realiza a soma da mesma forma que o 4-bit-adder, porem com uma porta a mais e uma saida a mais. Isso facilita o posicionamento em sequencia, fazendo assim um 8-bit-adder com mais facilidade.
### Entradas
- A e B: Uma entrada 4-bit que dara o valor positivo para soma.
- Carry in: Uma porta de 1-bit, que se refere a sobra que esta vindo de um calculo anterior.
### Saidas
- Sum: Valor que resulta a soma de A e B
- Carry Out: Valor que vem extrapolar e sobrar da soma realizada em A e B, sendo apenas simbolica ou necessaria para ser ligada ao carry in de outro 4-bit-adder.

## 8-bit-Adder-Scale
### Resumo
O circuito logico responsavel por realizar somas do tipo 8-bit, funciona da mesma forma que os outros Adder's.
### Entradas
- A e B: Uma entrada 8-bit que dara o valor positivo para soma.
- Carry in:  Uma porta de 1-bit, referente a sobra que esta vindo de um calculo anterior.
### Saidas
- Sum: Valor que resulta a soma de A e B
- Carry Out: Valor que vem extrapolar e sobrar da soma realizada em A e B, sendo apenas simbolica ou necessaria para ser ligada ao carry in de outro 8-bit-adder.

## Half-Substractor
### Entradas
- A: Minuendo
- B: Subtraendo de A
### Saidas
- Diff: Valor que resulta a subtracao entre A e B!
- Borrow: Valor que sera emprestado caso a casa de unidades do B seja maior que a do A!

## Full-Subtractor
### Resumo:
Borrow in e A farão uma primeira subtração que o resultado dessa conta, sera utilizada para outra subtração com o B e o valor de diff sera o resultado desse calculo, ja o borrow da primeira e da segunda conta caso eles deem algum valor sera expressado no borrow out.
### Entradas
- A: Minuentdo
- B: Subtraendo de A
- Borrow in: Subtraendo de A - B
### Saidas
- Diff: Valor da diff do primeiro half-substractor menos o segundo.
- Borrow out:  Se o valor do calculo realizado pelo half-substractor de A - borrow in for 1 ou caso o diff dessa conta menos B seja 1 este sera o valor representado pelo borrow out.