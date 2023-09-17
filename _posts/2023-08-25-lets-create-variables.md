---
layout: post
title: "Let's create variables"
tags: Python 
---

Chega de lenga-lenga (eu adoro as expressões da língua portuguesa) e vamos começar pra valer o aprendizado de Python.

Pra quem não viu, o Hello World já está [aqui nesse post](https://olimaandreza.github.io/2023/06/28/lets-understand-python.html).

E como prometido, 2 meses depois, o assunto de hoje é **Variáveis** (cumpri minha promessa de não ser 3 meses!).

## O que são variáveis?

Uma variável em python é uma maneira para guardar valores na memória do computador. O "Hello World" do código passado (`print("Hello World")`) foi processado apenas uma vez e seu valor não ficou guardado na memória. Ao se utilizar variáveis, o valor passa a ser armazenado e pode depois ser lido e manipulado a partir do nome definido para a variável sempre que for necessário.

A atribuição de variáveis em Python se dá pela seguinte fórmula, com o uso do operador `=`, assim:

> nomedavariavel = valor da variável

*Exemplo: criar uma variável chamada `a` com o valor 2:*

```py
a = 2
```

✨ Parabéns, você acabou de criar sua primeira variável!

Agora para imprimir o valor da variável, você já aprendeu a **função** `print()`:

```py
print(a)
```
o que vai imprimir na tela o seu valor: 2.

Se tentar imprimir `print("a")` no lugar de `print(a)`, o resultado será diferente. Mas por quê? Lembre-se sempre que se um valor está entre aspas, é considerado uma string, então será impresso o valor da própria string, similar ao que fizemos com o Hello World. Já o valor sem aspas sempre vai buscar na memória uma variável que tenha aquele nome.

## Alguns detalhes precisam de atenção

* Não há como declarar uma variável sem atribuir um valor inicial a ela.
* Os nomes das variáveis devem começar com uma letra ou um underline.
* O nome é *case sensitive*, isto significa que letras maiúsculas e minúsculas são diferentes (tente acessar o valor da variável `A`, por exemplo).
* A atribuição de variáveis funciona sempre da esquerda para a direita (valor = nomedavariavel não vai funcionar)
* Você não deve usar os comandos (keywords) do python como o nome de uma variável, sob risco de substituir comandos importantes. Por exemplo, uma variável não pode se chamar `print`, a função para imprimir valores na página.

>💡 Curiosidade:
>
> É possível atribuir valores a mais de uma variável por vez, usando a seguinte sintaxe (é necessário que se tenha o mesmo número de elementos antes e depois do sinal de igual que atribui valor às variáveis):
>
>   a, b, c =  1, 2, 3
>
>Também é possível atribuir um mesmo valor a várias variáveis de uma vez só:
>
>   a = b = c = None

## Tipos de variáveis

Existem vários tipos de dados que podem ser atribuídos às variáveis e isso impacta quais métodos (**funções**) podem ser usadas e qual o comportamento esperado desses dados.

Os tipos mais simples são:

* String: esse já conhecemos, é o caso do `"Hello world!"`, ou seja, um conjunto de caracteres que deve ser entendido como texto. Nada impede que um caracter numérico seja atribuído a uma String, basta que para isso seja informado entre aspas.

* Integer: na tradução, números inteiros, ou seja, qualquer número que não tenha casas decimais, são geralmente contagens de algo, mas podem ser positivos ou negativos.

* Float: número que tem casas decimais, mesmo que a casa decimal seja zero, por exemplo, `2` tem tipo diferente de `2.0`. Também podem ser positivos ou negativos.

* Boolean: aqui é onde as coisas começam a entrar na lógica computacional, mas basicamente esse tipo de variável assume apenas dois valores: verdadeiro ou falso (`True` ou `False`). Aqui eu quero que pense que uma variável booleana é como um interruptor que pode estar ligado ou desligado. É tipo o botão do elevador que você aperta para subir ou descer. Só que em programação, em vez de estar apertando um botão, é o computador que fica verificando se a luz está acesa ou apagada. E dependendo do resultado, seu programa pode fazer uma determinada ação. As variáveis booleanas são muito importantes em programação, porque elas ajudam a máquina a tomar decisões. Vamos falar mais sobre esse tipo mais na frente.

* None: Valor vazio ou com tipo de dados nulo

Lista, Tupla e Dicionário também são tipos de dados que podem ser armazenados em Python, mas esses ficam para um próximo post.

Ah! Você não precisa se preocupar em atribuir um tipo a uma variável, o próprio interpretador do Python (lembra do conceito de linguagem interpretada?) escolhe automaticamente o tipo mais adequado. Por isso Python também pode ser uma linguagem dinamicamente tipada: a depender do valor inserido, o interpretador seleciona o tipo e até pode alterá-lo, caso em um primeiro momento tenha atribuído uma string e depois um integer, por exemplo.

Para saber o tipo de uma variável, usa-se a **função** `type()`:

```py
type(a)
```
Resultado: int

Existem também várias funções que podem criar ou fazer a alteração do tipo de uma variável, por exemplo:

**Transforma em String:**

```py
string_a = str(a)
type(string_a)
```
Resultado: str

❔Desafio: o que você acha que vai acontecer ao executar `print(string_a)`?


**Transforma em float:**

```py
float_a = float(a)
type(float_a)
```
Resultado: float

❔Desafio: o que você acha que vai acontecer ao executar `print(float_a)`?

**Cria um int**
```py
a = int(2)
a
```
Resultado: 2


Para hoje, é isso. 
E assim, mais uma vez mergulhamos no universo de Python, explorando o conceito de variáveis, que são elementos fundamentais em qualquer análise de dados.

______

👉 Quem quiser, pode encontrar mais detalhes sobre os tipos de variáveis na documentação do Python: [https://docs.python.org/3/library/stdtypes.html](https://docs.python.org/3/library/stdtypes.html).



