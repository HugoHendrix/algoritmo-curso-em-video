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