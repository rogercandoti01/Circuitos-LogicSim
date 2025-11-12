# Circuitos-LogicSim
Yes
## 4-Bit-Adder
### Resumo
O circuito lógico é responsável por realizar a soma binária de dois números de 4 bits. Possui 1 half-adder, e 3 full-adder, onde o half faz os primeiros calculos e em sequencia os full-adder continuam utilizando os carrys dos calculos passados.
### Entradas
- A e B: Uma entrada 4-bit que dara um valor positivo para soma.
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