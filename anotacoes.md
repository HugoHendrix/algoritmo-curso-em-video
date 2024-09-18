# Iniciando o VisualG

Para criar uma estrutura inicial pressione `! + CTRL espaço `

```VisualG
algoritmo "semnome"
var
    //Área de variáveis

inicio

    // Corpo do Algoritmos

fimalgoritmo
``` 
---

### Comandos de saída 

- `Escreva ("Sua mensagem")` - Tudo dentro de aspas, são considerados strings ou seja cadeias de caracteres.
- `Escreval` - Semelhante ao escreva, mais com a letra L no final, utilizado para pular a linha de baixo.

``` VisualG
algoritmo "semnome"
var

inicio
escreval ("Olá, mundo")
escreva ("Já me livrei da maldição!")

fimalgoritmo
```
Para executar o algoritmo, dentro do Visualg, pressione F9

---

### Variáveis

O que é uma variável?
Imagine uma caixa com um rótulo. Dentro dessa caixa, você pode guardar qualquer tipo de coisa: uma bola, um livro, um brinquedo. A caixa representa uma variável na programação.

Em programação, uma variável é como um recipiente que armazena um valor. Esse valor pode ser um número, um texto, um valor lógico (verdadeiro ou falso), ou até mesmo uma estrutura de dados mais complexa.

---

### Identificadores em Portugol: Uma Explicação Detalhada

O que são identificadores?

Em programação, um identificador é um nome que você atribui a um elemento do seu programa, como uma variável, uma constante, uma função ou um procedimento. É como um rótulo que você coloca em algo para poder se referir a ele mais tarde.

Existem 6 regras para identificadores no Visualg:

* Deve começar com uma letra
* Os próximos podem ser letras ou números.
* Não se pode utilizar nenhum símbolo, exceto _
* Não pode conter espaços em branco
* Não pode conter letras com acentos
* Não pode ser uma palavra reservada (palavras utilizadas pelo sistema, por exemplo: algoritmo, var, inicio, fimalgoritmo etc).

---

### Tipos Primitivos

Em Portugol, assim como em outras linguagens de programação, os tipos primitivos são os tipos de dados mais básicos e fundamentais. Eles definem a natureza dos valores que uma variável pode armazenar.

Organização: Ajudam a organizar os dados de forma eficiente na memória do computador.
Operações: Cada tipo de dado suporta um conjunto específico de operações. Por exemplo, você pode somar dois números inteiros, mas não pode somar um número inteiro com uma letra.
Eficiência: O computador aloca a quantidade correta de memória para cada tipo de dado, otimizando o uso dos recursos.
Quais são os principais tipos primitivos em Portugol?

Os tipos primitivos mais comuns em Portugol são:

* Inteiro: Representa números inteiros, positivos ou negativos. Exemplo: idade, quantidade.
* Real: Representa números reais, ou seja, números com casas decimais. Exemplo: altura, peso, pi.
* Caractere: Representa um único caractere, como uma letra, um número ou um símbolo. Exemplo: letra, simbolo.
* Lógico: Representa valores lógicos, ou seja, verdadeiro (verdadeiro) ou falso (falso). Exemplo: condicao, resultado.

---

### Atribuições em Portugol: Atribuindo Valores a Variáveis

Em programação, uma atribuição é a ação de dar um valor a uma variável. É como colocar um número, uma palavra ou qualquer outro tipo de dado dentro de uma caixa (a variável).
A sintaxe básica para atribuir um valor a uma variável em Portugol é:

`VisualG nome_da_variavel <- valor;`

O símbolo **<-** é o operador de atribuição e significa **recebe**.

``` VisualG
algoritmo "semnome"
var
  msg: caractere

inicio
msg <- "Olá, mundo"
escreva (msg)

fimalgoritmo
``` 
Note que no escreva, foi retirado as aspas

### Comandos de saída

* Escreva("msg") - Vai escrever msg
* Escreva(msg) - Vai escrever o conteúdo da variável msg
* Escreva("mensagem", msg) - Vai exibir 2 coisas, vai escrever mensagem e o conteúdo da variável msg

```VisualG
algoritmo "semnome"
var
  msg: caractere

inicio
msg <- "Olá, mundo"
escreval ("Mensagem: ", msg)

fimalgoritmo
```