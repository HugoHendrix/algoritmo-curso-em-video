# Exercícios de Algoritmos - Professor Gustavo Guanabara

### 1 - Escreva um programa que mostre na tela a mensagem "Olá, mundo!"
```
algoritmo "ex01"
var

msg: caractere

inicio

msg <- "Olá, mundo!"
escreva (msg)

fimalgoritmo
```
---
### 2 - Faça um programa que leia o nome de uma pessoa e mostre uma mensagem de boas-vindas para ela:
Ex: 
Qual é o seu nome? João da Silva
Olá João da Silva, é um prazer te conhecer!

```
algoritmo "ex02"
var
nome: caractere
inicio
escreval ("Qual o seu nome?")
leia(nome)
escreval("Saudações, ", nome, " seja bem-vindo(a)")

fimalgoritmo
```
---
### 3 - Crie um programa que leia o nome e o salário de um funcionário, mostrando no final uma mensagem.
Ex:
Nome do Funcionário: Maria do Carmo
Salário: 1850,45
O funcionário Maria do Carmo tem um salário de R$1850,45 em Junho.

```
algoritmo "ex03"
var
nome: caractere
salario: real
inicio

nome <- "Maria do Carmo"
salario <- 1850.45
escreval ("A funcionaria ", nome, " tem um salario de", salario, " em Junho.")

fimalgoritmo
``` 
---

### 4 - Desenvolva um algoritmo que leia dois números inteiros e mostre o somatório entre eles.
Ex:
Digite um valor: 8
Digite outro valor: 5
A soma entre 8 e 5 é igual a 13.
```
algoritmo "ex04"
var

n1, n2, r: inteiro

inicio

n1 <- 8
n2 <- 5
r <- n1 + n2

escreva ("A soma entre ",n1, " e ", n2, " é igual a ", r)

fimalgoritmo
```

---

### 5 - Faça um programa que leia as duas notas de um aluno em uma matéria e mostre na tela a sua média na disciplina.
Ex:
Nota 1: 4.5
Nota 2: 8.5
A média entre 4.5 e 8.5 é igual a 6.5
```
Algoritmo "calcularMedia"

Var

n1, n2, media: real

Inicio

escreval("Digite sua nota: ")
leia(n1)
escreval("Digite sua outra nota: ")
leia(n2)
media <- (n1 + n2) /2
escreval("A média entre a nota ", n1," e ",n2, " é igual a ", media )

Fimalgoritmo
```
---

### 6 - Faça um programa que leia um número inteiro e mostre o seu antecessor e seu sucessor.
Ex:
Digite um número: 9
O antecessor de 9 é 8
O sucessor de 9 é 10
```
algoritmo "antecessorSucessor"
var

antecessor, sucessor, numero: inteiro

inicio

escreval("Digite um número: ")
leia(numero)
antecessor <- numero -1
escreval ("O numero informado foi ",numero," seu antecessor é", antecessor)
sucessor <- numero +1;
escreval("O numero informado foi ",numero," seu sucessor é", sucessor)

fimalgoritmo
```
---

### 7 - Crie um algoritmo que leia um número real e mostre na tela o seu dobro e a sua terça parte.
Ex:
Digite um número: 3.5
O dobro de 3.5 é 7.0
A terça parte de 3.5 é 1.16666
```
algoritmo "dobroTerco"
var

numero, dobro, terco: real

inicio

escreval("Digite um número: ")
leia(numero)
dobro <- numero * 2
escreval("O número informado foi ", numero, ", o dobro desse número é ", dobro)
terco <- numero / 3
escreval("O número informado foi ", numero, " a terça parte desse número é ", terco:2:4)

fimalgoritmo
```
---
### 8 - Desenvolva um programa que leia uma distância em metros e mostre os valores relativos em outras medidas.
Ex:
Digite uma distância em metros: 185.72
A distância de 85.7m corresponde a:
0.18572Km
1.8572Hm
18.572Dam
1857.2dm
18572.0cm
185720.0mm
```
algoritmo "calcularDistancia"
var

valorMetros: real
valorKm: real
valorHm: real
valorDam: real
valorDm: real
valorCm: real
valorMm: real

inicio
escreval ("Digite um valor em metros: ")
leia(valorMetros)
valorKm <- valorMetros / 1000
escreval ("O valor digitado em metros foi", valorMetros, " convertido para Quilômetro, passa a ser:", valorKm," KM")
valorHm <- valorMetros /100
escreval ("O valor digitado em metros foi,", valorMetros, " convertido para Hectômetro, passa a ser: ", valorHm," HM")
valorDam <- valorMetros /10
escreval ("O valor digitado em metros foi,", valorMetros, " convertido para Decâmetro, passa a ser: ", valorDam," DAM")
valorDm <- valorMetros * 10
escreval("O valor digitado em metros foi ", valorMetros, " convertido para Decímetro, passa a ser: ", valorDm," DM")
valorCm <- valorMetros * 100
escreval("O valor digitado em metros foi ", valorMetros, " convertido para Cemtímetros, passa a ser: ", valorCm," CM")
valorMm <- valorMetros * 1000
escreval("O valor digitado em metros foi ", valorMetros, "convertido para Milímetro, passa a ser: ", valorMm," MM")
fimalgoritmo 
```
---
### 9 - Faça um algoritmo que leia quanto dinheiro uma pessoa tem na carteira (em R$) e mostre quantos dólares ela pode comprar. Considere US$1,00 = R$3,45.
```
algoritmo "conversorDolar"
var

valorReal: real
valorDolar: real

inicio
escreval ("Quantos reais você tem para converter em dolar? ")
leia(valorReal)
valorDolar <- valorReal * 3.45
escreval("O valor digitado em reais foi: ", valorReal, ", convertido para dolar, o valor passa a ser: R$:", valorDolar:2:2)

fimalgoritmo
```
---
### 10 - Faça um algoritmo que leia a largura e altura de uma parede, calcule e mostre a área a ser pintada e a quantidade de tinta necessária para o serviço, sabendo que cada litro de tinta pinta uma área de 2 metros quadrados.
```
algoritmo "calculaArea"
var

paredeAltura: real
paredeLargura: real
litroTinta: real
areaTotal: real

inicio
escreval ("Por favor digite a altura da parede: ")
leia(paredeAltura)
escreval("Por favor digite a largura da parece: ")
leia(paredeLargura)
areaTotal <- paredeAltura * paredeLargura
escreval("A altura da parede é ", paredeAltura, " metros, a largura da parede, é ", paredeLargura, " metros, o total da área é ", areaTotal, " metros")
litroTinta <- areaTotal / 2
escreval("Para pintar a área de", areaTotal, " metros, será necessário ", litroTinta, " litros de tinta")


fimalgoritmo
```
---
### 11 - Desenvolva uma lógica que leia os valores de A, B e C de uma equação do segundo grau e mostre o valor de Delta.
```
algoritmo "calculaDelta"
var

a, b, c, delta: real

inicio
escreval ("Digite o valor de a: ")
leia(a)
escreval ("Digite o valor de b: ")
leia(b)
escreval ("Digite o valor de c: ")
leia(c)
delta <- b^2 - 4*a*c
escreval("O valor de delta é: ", delta)
fimalgoritmo
```
---
### 12 -  Crie um programa que leia o preço de um produto, calcule e mostre o seu PREÇO PROMOCIONAL, com 5% de desconto.
```
algoritmo "calcularDesconto"
var

precoProduto: real
desconto: real
precoPromocao: real

inicio
escreval("Digite o valor do produto: ")
leia(precoProduto)
desconto <- precoProduto * 0.05  // Calculando o valor do desconto (5% de precoProduto)
precoPromocao <- precoProduto - desconto  // Calculando o preço com desconto
escreval("O valor do produto é ", precoProduto, " com desconto de 5%, o valor agora é: ", precoPromocao)

fimalgoritmo
```
---
### 13 - Faça um algoritmo que leia o salário de um funcionário, calcule e mostre o seu novo salário, com 15% de aumento.
```
algoritmo "aumentaSalario"
var

salarioAtual: real
aumento: real
salarioAumento: real

inicio
escreval("Digite seu salário atual: ")
leia(salarioAtual)
aumento <- salarioAtual * 0.15
salarioAumento <- salarioAtual + aumento

escreval("Com o aumento seu salário é: ", salarioAumento)

fimalgoritmo
```
---
### 14 - A locadora de carros precisa da sua ajuda para cobrar seus serviços. Escreva um programa que pergunte a quantidade de Km percorridos por um carro alugado e a quantidade de dias pelos quais ele foi alugado. Calcule o preço total a pagar, sabendo que o carro custa R$90 por dia e R$0,20 por Km rodado.
```
algoritmo "alugaCarro"
var

diasAlugados, kmPercorrido: inteiro
valorPorDia, valorPorKm, valorDias, valorKm, valorTotal: real

inicio
escreval("Informe a quantiddade de dias alugados: ")
leia(diasAlugados)
escreval("Informe a quantidade de quilômentros percorridos: ")
leia(kmPercorrido)
valorPorDia <- 90.00
valorKm <- 0.20

valorDias <- diasAlugados * valorPordia
valorPorKm <- kmPercorrido * valorKm
valorTotal <- valorDias + valorPorKm
escreval("O valor total a pagar é: R$",valorTotal:2:2)

fimalgoritmo
```
---

### 15 -  Crie um programa que leia o número de dias trabalhados em um mês e mostre o salário de um funcionário, sabendo que ele trabalha 8 horas por dia e ganha R$25 por hora trabalhada.
```
algoritmo "salarioFuncionar"

var
diasTrabalhados, horasTrabalhadas: inteiro
valorHora, salario: real

inicio
escreval("Informe a quantidade de dias trabalhados no mês: ")
leia(diasTrabalhados)

valorHora <- 25
horasTrabalhadas <- diasTrabalhados * 8
salario <- horasTrabalhadas * valorHora
escreval("O salário do funcionário é RS:",salario:2:2)

fimalgoritmo
```
---
