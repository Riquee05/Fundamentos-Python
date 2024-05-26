## Estruturas Condicionais
if, elif, else

Estas estruturas são usadas para executar blocos de código com base em condições específicas.

Sintaxe básica:

1. python

        if condição:
        bloco de código executado se a condição for verdadeira
        elif outra_condição:
        bloco de código executado se a outra_condição for verdadeira
        else:
    bloco de código executado se nenhuma das condições anteriores for verdadeira

Exemplo:

### python

    idade = 18

    if idade < 18:
        print("Menor de idade")
    elif idade == 18:
        print("Tem 18 anos")
    else:
        print("Maior de idade")

    Estruturas de Repetição
    for

A estrutura for é usada para iterar sobre uma sequência (como uma lista, tupla, string) ou qualquer outro objeto iterável.

Sintaxe básica:

python

    for elemento in iterável:
        # bloco de código a ser executado para cada elemento

    Exemplo:

    python

    frutas = ["maçã", "banana", "cereja"]

    for fruta in frutas:
        print(fruta)

    Iterando com range():

    python

    for i in range(5):
        print(i)

while

A estrutura while continua executando o bloco de código enquanto a condição for verdadeira.

Sintaxe básica:

    python

    while condição:
        # bloco de código a ser executado enquanto a condição for verdadeira

    Exemplo:

    python

    contador = 0

    while contador < 5:
        print(contador)
        contador += 1

Controle de Fluxo em Estruturas de Repetição
break

O break é usado para sair de um loop imediatamente, independentemente da condição do loop.

Exemplo:

python

    for i in range(10):
        if i == 5:
            break
        print(i)

continue

O continue faz com que o loop pule o restante do bloco de código e vá para a próxima iteração.

Exemplo:

python

    for i in range(10):
        if i % 2 == 0:
            continue
        print(i)

else com Loops

Em Python, os loops for e while podem ter um bloco else que é executado quando o loop termina normalmente (não por um break).

Exemplo com for:

python

    for i in range(5):
        print(i)
    else:
        print("Loop terminou normalmente")

Exemplo com while:

python

    contador = 0

    while contador < 5:
        print(contador)
        contador += 1
        else:
        print("Loop terminou normalmente")

Essas estruturas fornecem um controle robusto sobre o fluxo do programa, permitindo a execução condicional e repetitiva de blocos de código com base em diferentes condições e cenários.



