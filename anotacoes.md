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

### Comando de Entrada e Operadores

Comandos de Entrada:

leia: Captura dados do usuário e armazena em uma variável.
Exemplo: leia(idade);

**Operadores:**

* Aritméticos: Realizam cálculos (soma, subtração, multiplicação, divisão, módulo).
  - Exemplo: resultado <- numero1 + numero2;
* Relacionais: Comparam valores (igual, diferente, maior, menor).
  - Exemplo: se idade >= 18 entao
* Lógicos: Combinam condições lógicas (e, ou, não).
  - Exemplo: se (temCarteira && idade >= 18) entao

Em resumo:

Comandos de entrada: Interagem com o usuário.
Operadores: Realizam operações em valores.

```VisualG
algoritmo "meuNome"
var
   nome: caractere
   idade: inteiro

inicio

      escreval ("Digite seu nome?")
      Leia(nome)
      escreval ("Muito prazer, ", nome)
      escreval ("Qual a sua idade?")
      leia (idade)
       se idade >= 18 entao
      escreva(nome, ", você é maior de idade.")
       senao
      escreva(nome, ", você é menor de idade.")
      fimse
fimalgoritmo
```

### Exercício de somar valores

```Visualg
algoritmo "somarNumeros"
var
n1, n2, resultado: inteiro
inicio
escreva ("Infome um número: ")
leia(n1)
escreva ("Inforem outro número: ")
leia(n2)
resultado <- n1 + n2
escreval ("A soma entre o número ", n1, " e o número ", n2," é igual a ", resultado)

fimalgoritmo
``` 
---

### Operadores Aritméticos em Portugol
Operadores aritméticos são símbolos utilizados para realizar cálculos matemáticos básicos. Em Portugol, os principais são:

+: Adição
-: Subtração
*: Multiplicação
/: Divisão
\: Divisão inteira
^: Exponenciação
%: Módulo (resto da divisão)

```VisualG
algoritmo "semnome"
var

a, b, resultadoSomar, resultadoSubtrair, resultadoMultiplicacao: inteiro
resultadoDivisao, resultadoExponenciacao, resultadoModulo: real

inicio

escreva("Digite um número: ")
leia(a)
escreva("Digite outro número: ")
leia(b)
escreval("Os números informados foram ",a," e ", b)
resultadoSomar <- a + b
resultadoSubtrair <- a - b
resultadoMultiplicacao <- a * b
resultadoDivisao <- a / b
resultadoExponenciacao <- a ^ b
resultadoModulo <- a % b
escreval("A soma entre os números informados, são: ",resultadoSomar)
escreval("A subtração entre os números informados, são: ",resultadoSubtrair)
escreval("A multiplicalçao entre os números informados, são: ",resultadoMultiplicacao)
escreval ("A divisão entre os números informados, são: ",resultadoDivisao)
escreval ("A exponenciação entre os número informados, são: ",resultadoExponenciacao)
escreval ("O resto da divisão entre os números informados, são: ",resultadoModulo)
fimalgoritmo
```
---

### Ordem de Precedência em Operadores Aritméticos

A ordem em que as operações são realizadas em uma expressão matemática segue uma regra chamada ordem de precedência.

A ordem é a seguinte:
() PARÊNTESES
^ EXPONENCIAÇÃO
* / MULTIPLICAÇÃO E DIVISÃO
+- ADIÇÃO E SUBTRAÇÃO 

Parênteses: Tudo dentro de parênteses é calculado primeiro.
Multiplicação e Divisão: São realizadas antes da adição e subtração.

Adição e Subtração: São realizadas por último.
`resultado <- 2 + 3 * 4; // Resultado é 14 (3*4 primeiro)`

Para mudar a ordem, use parênteses:
`resultado <- (2 + 3) * 4; // Resultado é 20`

### Exercício de Cálcula de Média

```VisualG
algoritmo "semnome"
var

n1, n2: inteiro
media: real

inicio
escreva ("Informe um número: ")
leia(n1)
escreva ("Informe outro número: ")
leia(n2)
media <- (n1 + n2) / 2
escreva ("A media entre ",n1, " e ",n2," é igual ", media)

fimalgoritmo
```

### Funções Aritméticas 23:09

