### Iniciando o VisualG

Para criar uma estrutura inicial pressione `! + CTRL espaço `

```VisualG
algoritmo "semnome"
var
    //Área de variáveis

inicio

    // Corpo do Algoritmos

fimalgoritmo
``` 

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

# Variáveis

### O que é uma variável?
Imagine uma caixa com um rótulo. Dentro dessa caixa, você pode guardar qualquer tipo de coisa: uma bola, um livro, um brinquedo. A caixa representa uma variável na programação.

Em programação, uma variável é como um recipiente que armazena um valor. Esse valor pode ser um número, um texto, um valor lógico (verdadeiro ou falso), ou até mesmo uma estrutura de dados mais complexa.

### Identificadores em Portugol: Uma Explicação Detalhada

O que são identificadores?

Em programação, um identificador é um nome que você atribui a um elemento do seu programa, como uma variável, uma constante, uma função ou um procedimento. É como um rótulo que você coloca em algo para poder se referir a ele mais tarde.

Existem 6 regras para identificadores no Visualg:

* - Deve começar com uma letra
* - Os próximos podem ser letras ou números.
* - Não se pode utilizar nenhum símbolo, exceto _
* - Não pode conter espaços em branco
* - Não pode conter letras com acentos
* - Não pode ser uma palavra reservada (palavras utilizadas pelo sistema, por exemplo: algoritmo, var, inicio, fimalgoritmo etc).