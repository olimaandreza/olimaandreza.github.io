---
layout: post
title: "Let's understand Python"
tags: Python
---

Honrando a descrição do blog: como eu não sei ser blogger, quase 3 meses depois, chega um novo post. Hoje me senti inspirada para postar: estou participando do processo seletivo Santander Coders 2023 na trilha de engenharia de dados e uma das etapas é justamente um Coding Tank com os primeiros passos em Python, e é sobre isso que vim falar hoje.

Então, um overview.

Python é uma linguagem de programação que os humanos podem usar para escrever instruções para o computador executar tarefas específicas.

É definida como uma linguagem de programação de alto nível, interpretada e orientada a objetos. Mas vamos por partes:

*Python é uma linguagem de programação de alto nível...*

Isso significa que foi projetada para ser fácil de entender e escrever para os humanos, em contraste com as linguagens de baixo nível, que são projetadas para serem entendidas mais diretamente pelo computador.

*Python é uma linguagem de programação interpretada...*

Isso significa que as instruções (linhas de código do programa) são lidas e executadas linha por linha diretamente pelo computador, sem haver a necessidade de passar por um processo de compilação, isto é, um processo de transformação da linguagem de alto nível para uma linguagem de baixo nível que o computador entende (esse conceito você já aprendeu!).

*Python é uma linguagem de programação orientada a objetos...*

Esse para mim é o mais difícil de explicar, quem tiver outra forma, me ajuda aí! 

Mas é mais ou menos o seguinte: uma linguagem de programação orientada a objetos permite a criação de estruturas de atributos que podem ser facilmente reutilizadas em diferentes partes de um programa. Em outras palavras, em vez de escrever um código complexo repetidamente, você pode criar um objeto que contenha todas as informações e funcionalidades necessárias e, em seguida, usar esse objeto sempre que precisar dele.

## Hello world

O "Hello, World!" é considerado uma tradição na programação de computadores e é usado como um rito de passagem para muitos programadores iniciantes. O objetivo é criar um programa que imprime a frase "Hello, World!" na tela do computador.

Em python, a função `print()` vai fazer esse trabalho. Sempre que quiser imprimir um resultado na tela, print() vai ser sua melhor amiga.

Para imprimir um texto, coloque-o entre aspas, e o resultado será impresso na tela.  Tenta aí:

    print("Hello World!")

Pronto, parabéns, você fez seu primeiro programa em Python.

Mas lembre: Ao utilizar a função print para imprimir valores que são um texto, precisamos sempre indicar para o programa com o uso de aspas, caso contrário, ele vai procurar na memória uma **variável** com o nome do texto inserido, e isso pode acarretar um erro ou resultados não previstos. Ou seja, cuidado: `print("Hello")` é diferente de `print(Hello)`.

E por falar em variáveis, esse vai ser o tema do próximo post de Python.