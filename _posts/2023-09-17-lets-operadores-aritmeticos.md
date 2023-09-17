---
layout: post
title: "Let's explore arithmetic operators "
tags: Python
---

Olá, data lovers! Bem-vindos ao "All We Need is Data!". Hoje o assunto é mamão com açúcar, apesar de ser um aspecto fundamental de qualquer linguagem de programação: os operadores aritméticos, esses pequenos símbolos mágicos que nos permitem realizar uma série de cálculos matemáticos e manipular dados de maneiras poderosas. 

Vamos ver como fazer isso com Python.

## Operadores básicos: +  -  *  /

Sem mistério. Quer somar dois números em Python? Simples, use o operador `+`. Subtrair? Use `-`. Para multiplicar, `*` e para dividir, `/`. Segue aí:

```py 
## Soma:
3+1
# Output: 4

## Subtração
3-1
# Output: 2

## Multiplicação
3*3
# Output: 9

## Divisão
6/3
# Output: 2.0
```

Aqui, cabe uma observação: a divisão sempre vai gerar um resultado do tipo float, o que pode ser verificado com a função `type()`:

```py
type(6)
# Output: int

type(3)
# Output: int

type(6/3)
# Output: float
```
💡 Quer rever o conteúdo de variáveis? [Clique aqui](https://olimaandreza.github.io/2023/08/25/lets-create-variables.html).

## Exponencial, raiz, divisão inteira e módulo: ** // %

Agora, vamos falar sobre alguns operadores menos usuais no dia-a-dia e também menos intuitivos, mas igualmente simples na notação. Começando pelo exponencial e raiz quadrada, para os quais usamos o mesmo operador `**`, pois a raiz quadrada nada mais é do que elevar um número a 1/2.

```py
## Exponencial
2**3
# Output: 8

## Raiz
4**(1/2)
# Output: 2.0
```

Observe que o resultado de uma exponencial fracionária gera como resultado um float.

Para finalizar, tenho apenas mais dois operadores para falar.

Primeiro, para obter apenas a **parte inteira** de uma divisão: operador `//`

```py
5 // 2
# Output: 2
```

Aqui, apesar de envolver uma divisão, o resultado é do tipo inteiro, conforme a própria definição do operador. A parte fracionária é desprezada.

E em seguida, para obter o **resto** dessa divisão: operador `%` (também chamado de módulo)

```py
5 % 2 
# Output: 1
```

Pronto, você já aprendeu os operadores aritméticos em Python, falei que ia ser fácil! Mas falta ainda um detalhe muito importante: em uma aplicação na vida real, você pode precisar realizar vários cálculos em uma mesma variável, e para isso é preciso ter atenção à **ordem de precedência** dos operadores.

Isso significa que, quando se tem expressões com vários operadores, a linguagem Python segue uma sequência definida para calcular o resultado final. Essa sequência é:

1. Parênteses `()`: Igual nas aulas de matemática, qualquer operação dentro de parênteses é executada primeiro em Python. Isso permite um controle explícito da ordem de execução.

2. Exponenciação `**`: depois dos parênteses, a execução da expressão procura por operadores de exponenciação, da esquerda para a direita.

3. Multiplicação `*`, Divisão `/`, Divisão Inteira `//` e Módulo `%`: Essas operações são executadas da esquerda para a direita. Se tiver várias delas na mesma expressão, elas são avaliadas na ordem em que aparecem.

4. Adição `+` e Subtração `-`: As últimas operações a serem avaliadas são a adição e a subtração que, da mesma forma que a multiplicação e a divisão, também são executadas da esquerda para a direita, na ordem em que aparecem na expressão.

E agora, você consegue me dizer o resultado da expressão: `4*2+5-20/2**2`?

## Operadores aritméticos com Strings

É isso mesmo, você não leu errado! Dois operadores aritméticos podem ser aplicados a Strings, e seu uso é igualmente intuitivo. São eles a adição e a multiplicação, que realizam respectivamente as ações de concatenar e repetir uma string.

Vamos com calma.

Concatenação (`+`): O operador de adição `+` pode ser usado para unir (concatenar) duas ou mais strings. Ele simplesmente junta as strings na ordem em que aparecem. Exemplo:

```py
"Olá, " + "mundo!"
# Output: Olá, mundo!
```

Repetição (`*`): O operador de multiplicação `*` pode ser usado para repetir uma string várias vezes. Ele multiplica a string pelo número de vezes especificado.

```py
"olá" * 3
# Output: oláoláolá
```
_____

Bom, pra hoje é isso. Me despeço reforçando que a habilidade de manipular números e dados é essencial em programação, e esses operadores são ferramentas-chave para executar cálculos e operações matemáticas em seus projetos. E de brinde, ainda vimos como usar alguns operadores com Strings, fechando com chave de ouro.


