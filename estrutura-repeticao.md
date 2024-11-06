# Entendendo as Estruturas de Repetição

As estruturas de repetição são ferramentas poderosas na programação, permitindo que um bloco de código seja executado repetidamente enquanto uma determinada condição for verdadeira. No Portugol Visualg, temos os comandos `Enquanto`, `Repita` e `Para` para implementar essas repetições.

- **Enquanto (While)**: Executa um bloco de comandos enquanto uma condição for verdadeira. A verificação da condição ocorre no início do loop.
- **Repita (Do-While)**: Executa um bloco de comandos pelo menos uma vez e continua a repetição enquanto uma condição for verdadeira. A verificação da condição ocorre no final do loop.
- **Para (For)**: Executa um bloco de comandos um número determinado de vezes. É utilizado quando se conhece antecipadamente o número de iterações.

### Exemplo utilizando Enquanto
```Portugol Portugol Visualg
algoritmo "ContarAte10"
var

Contador: Inteiro

inicio

Contador <- 1
         Enquanto (Contador <= 10 ) Faca
                  Escreval(Contador)
                  Contador <- Contador + 1
         FimEnquanto

fimalgoritmo
```
---

### Exemplo utilizando Repita
```Portugol Portugol Visualg
algoritmo "ContarAte10"
var

Contador: Inteiro

inicio

Contador <- 1
         Repita
                  Escreval(Contador)
                  Contador <- Contador + 1
         Ate (Contador > 10)


fimalgoritmo
```
---

### Exemplo utilizando Para
```Portugol Portugol Visualg
algoritmo "ContarAte10"
var

Contador: inteiro

inicio

    Para Contador <- 1 ate 10 Faca
        Escreval(Contador)
    FimPara

fimalgoritmo
```

### Quando Usar Cada Estrutura?
- Enquanto: Ideal para situações em que não se sabe exatamente quantas vezes o loop será executado, mas se tem uma condição de parada.
- Repita: Utilizado quando se deseja que o bloco de comandos seja executado pelo menos uma vez, independentemente da condição inicial.
- Para: Empregado quando se conhece o número exato de iterações que serão realizadas.

### Dicas para Utilizar as Estruturas de Repetição
- Indentação: Utilize a indentação corretamente para delimitar o bloco de comandos que será repetido.
- Condição de parada: Defina uma condição de parada clara para evitar loops infinitos.
- Variável de controle: Utilize uma variável para controlar o número de iterações, especialmente em loops Para.
- Escolha a estrutura adequada: Analise o problema e escolha a estrutura de repetição que melhor se adapta à sua lógica.

----

# Exercícios Estruturas de Repetição 

## Usando Enquanto

### Prática 01 - Contador de 0 a 10

```Portugol Portugol Visualg
algoritmo "ContarAte10"
var
  contador: Inteiro

inicio
  contador <- 0
  enquanto (contador <= 10) faca
    Escreval(contador)
    contador <- contador + 1
  fimenquanto
fimalgoritmo
```

---

### Subtraindo de 100 a 1 (de 10 em 10)

```Portugol Portugol Visualg
algoritmo "Subtrair"
var
  contador: Inteiro

inicio
  contador <- 100
  enquanto (contador >= 1) faca
    Escreval(contador)
    contador <- contador - 10
  fimenquanto
fimalgoritmo
```

---

### Contar até o número inserido pelo usuário

```Portugol Portugol Visualg
algoritmo "ContarAteQuantos?"
var
  valor, contador: Inteiro

inicio
  contador <- 0
  escreval("Olá, quer contar até qual número? ")
  leia(valor)
  enquanto (contador <= valor) faca
    Escreval(contador)
    contador <- contador + 1
  fimenquanto
fimalgoritmo
```

---

### Contar até o número inserido com salto definido pelo usuário

```Portugol Portugol Visualg
algoritmo "ContarAteQuantosComSalto"
var
  valor, salto, contador: Inteiro

inicio
  contador <- 0
  escreval("Olá, quer contar até qual número? ")
  leia(valor)
  escreval("Qual o valor do salto?")
  leia(salto)
  enquanto (contador <= valor) faca
    Escreval(contador)
    contador <- contador + salto
  fimenquanto
fimalgoritmo
```

---

### Somador Numérico (maior, menor e soma dos valores inseridos)

```Portugol Portugol Visualg
algoritmo "SomadorNumerico"
var
  contador, valor, soma, maiorNumero, menorNumero: inteiro

inicio
  contador <- 1
  soma <- 0

  escreva("Digite o 1o. valor: ")
  leia(valor)
  maiorNumero <- valor
  menorNumero <- valor
  soma <- valor
  contador <- 2

  enquanto (contador <= 5) faca
    escreva("Digite o ", contador, "o. valor: ")
    leia(valor)

    se (valor > maiorNumero) entao
      maiorNumero <- valor
    fimse

    se (valor < menorNumero) entao
      menorNumero <- valor
    fimse

    soma <- soma + valor
    contador <- contador + 1
  fimenquanto

  Escreval("A soma dos números informados foi de ", soma)
  Escreval("O maior número informado foi ", maiorNumero)
  Escreval("O menor número informado foi ", menorNumero)
fimalgoritmo
```

---

### Conversor de Moedas
```Portugol Visualg
algoritmo "ConversorDeMoedas"
var

reais, dolares: real

inicio

Escreval ("Qual o valor será convertido em dolares americanos? ")
Leia(reais)
dolares <- reais / 5.40
Escreval("O valor informado de", reais, " reais, convertido em dolares, será: ", dolares:2:2)

fimalgoritmo
```

### Conversor de Moedas com quantidade de conversões
```Portugol Visualg

algoritmo "Convesor"
var

reais, dolares: real
contador, numeroConversoes: inteiro

inicio

contador <- 1
numeroConversoes <- 1
Escreval("Quantas conversões serão realizadas? ")
Leia (numeroConversoes)
Enquanto (contador <= numeroConversoes) Faca
         Escreval("Qual o valor em R$? ")
         Leia(reais)
         dolares <- reais /5.40
         Escreval("O valore convertido é US$ ", dolares:5:2)
         contador <- contador + 1


FimEnquanto
fimalgoritmo
```

## Estrutura de Repetição usando Repita

### Somando Números
```Portugol Visualg
algoritmo "SomandoNumeros"
var
N, S: Inteiro
Resp: Caractere

inicio

      S <- 0
      Repita
               Escreva ("Digite o valor ==> ")
               Leia (N)
               S <- S + N
               Escreva ("Você quer continuar ? [S/N] ")
               Leia (Resp)
      Ate (Resp = "n")
      Escreval("A soma de todos os valores é: ", s)

fimalgoritmo
```
---

### Contar até 10

```Portugol Visualg
algoritmo "contarAte10"
var

Cont: Inteiro

inicio
      Cont <- 1
      Repita
            Escreval(Cont)
            Cont <- Cont + 1
      Ate (Cont > 10)


fimalgoritmo
```

---

### Taboada Express

```Portugol Visualg
algoritmo "TabuadaExpress"
var

Taboada, Resultado, Numero, Contador: Inteiro

inicio
      Contador <- 1
      Escreval("Bem vindo ao Tabuada Express")
      Escreval("Qual número você quer ver a tabuada?")
      Leia(Numero)
      Repita
            Resultado <- Numero * Contador
            Escreval(Numero, " X ", Contador, " = ", Resultado)
            Contador <- Contador + 1
      Ate (Contador > 10)


fimalgoritmo
```

---

### Contar Número Negativos

```Portugol Visualg
algoritmo "ContaNegativos"
var

  C, N, TotN: Inteiro

inicio
      C <- 1
      Repita
            Escreva ("Digite um número: ")
            Leia (N)
            Se (N < 0 ) Entao
               TotN <- TotN + 1
            FimSe
            C <- C + 1
       Ate (C > 5)
       Escreval ("Foram digitados ", TotN, " valores negativos")
            

fimalgoritmo
```

---

### Calcular Fatorial

```Portugol Visualg
algoritmo "CalcularFatorial"
var

   Numero, Fatorial, Contador: Inteiro

inicio

Escreval ("Digite um número ")
Leia(Numero)
Contador <- Numero
Fatorial <- 1
Repita
      Fatorial <- Fatorial * Contador
      Contador <- Contador - 1
Ate (Contador < 1)
Escreva ("O valor do Fatorial de ", Numero, " é igual a ", Fatorial)

fimalgoritmo
```

---

### Calcular Fatorial com vários números com opção de contiuar ou não

```Portugol Visualg
algoritmo "CalcularFatorial"
var

   Numero, Fatorial, Contador: Inteiro
   Resposta: Caractere

inicio
Repita
      Escreval ("Digite um número ")
      Leia(Numero)
      Contador <- Numero
      Fatorial <- 1
      Repita
            Fatorial <- Fatorial * Contador
            Contador <- Contador - 1
      Ate (Contador < 1)
      Escreval ("O valor do Fatorial de ", Numero, " é igual a ", Fatorial)
      Escreval ("Quer continuar? [S/N]")
      Leia(Resposta)
Ate (Resposta = "n")
LimpaTela

fimalgoritmo
```

---

### Calcular Número Primo

```Portugol Visualg
algoritmo "NumeroPrimo"
var

ContDiv, Contador, Numero: Inteiro

inicio
      Contador <- 1
      ContDiv <- 0
      Escreval ("Digite um número: ")
      Leia(Numero)
      Repita
            Se (Numero % Contador = 0) Entao
               ContDiv <- ContDiv + 1
            FimSe
            Contador <- Contador + 1
      Ate (Contador > Numero )
      Se (ContDiv > 2) Entao
            Escreval("O valor ", Numero, " não é um número primo")
      SeNao
           EscrevaL("O valor ", Numero, " é um número primo!")
      FimSe

fimalgoritmo
```

---

### Calcula Número Primo com opção de continuar ou não

```Portugol Visualg

algoritmo "NumeroPrimo"
var

ContDiv, Contador, Numero: Inteiro
Resposta: Caractere

inicio
Repita
      Contador <- 1
      ContDiv <- 0
      Escreval ("Digite um número: ")
      Leia(Numero)
      Repita
            Se (Numero % Contador = 0) Entao
               ContDiv <- ContDiv + 1
            FimSe
            Contador <- Contador + 1
      Ate (Contador > Numero )
      Se (ContDiv > 2) Entao
            Escreval("O valor ", Numero, " não é um número primo")
      SeNao
           EscrevaL("O valor ", Numero, " é um número primo!")
      FimSe
      Escreval ("Quer continuar? [S/N]")
      Leia(Resposta)
Ate (Resposta = "n")
LimpaTela

fimalgoritmo
```
--- 

## Estrutura de Repetição utilizando Para

### Contando até 10

```Portugol Visualg
algoritmo "ContarAte!0"
var

Contador: Inteiro

inicio
      Para Contador <- 1 Ate 10 Faca
           Escreval(Contador)
      FimPara

fimalgoritmo
```
---

### Contando até 10 pulando de 2 em 2

```
algoritmo "ContarAte!0"
var

Contador: Inteiro

inicio
      Para Contador <- 1 Ate 10 passo 2 Faca
           Escreval(Contador)
      FimPara

fimalgoritmo
```

---

### Números Pares

```Portugol Visualg
algoritmo "valoresPares"
var
   Contador, Valor: Inteiro

inicio

      Escreva("Digite um valor: ")
      Leia(Valor)
      Para Contador <- 0 Ate Valor Passo 2 Faca
           Escreval(Contador)
      FimPara

fimalgoritmo
```

---