Em Python, listas são coleções ordenadas e mutáveis que permitem armazenar múltiplos itens em uma única variável. Listas podem conter itens de diferentes tipos, incluindo outras listas.

Aqui está um guia abrangente sobre listas em Python:
Criando uma Lista

Você pode criar uma lista usando colchetes [] ou a função list().

python

    # Criando uma lista vazia
    minha_lista = []

    # Criando uma lista com elementos
    minha_lista = [1, 2, 3, 4, 5]

    # Usando a função list()
    outra_lista = list([6, 7, 8, 9, 10])

Acessando Elementos

Elementos em uma lista são acessados usando índices, que começam em 0.

python

    minha_lista = [10, 20, 30, 40, 50]

    # Primeiro elemento
    print(minha_lista[0])  # Output: 10

    # Último elemento
    print(minha_lista[-1])  # Output: 50

    # Sublista
    print(minha_lista[1:3])  # Output: [20, 30]

Modificando Elementos

Você pode modificar elementos diretamente acessando-os pelo índice.

python

    minha_lista = [1, 2, 3, 4, 5]
    minha_lista[2] = 30  # Alterando o terceiro elemento
    print(minha_lista)  # Output: [1, 2, 30, 4, 5]

    Adicionando Elementos

        append(): Adiciona um único elemento ao final da lista.
        insert(): Insere um elemento em uma posição específica.
        extend(): Adiciona múltiplos elementos de outra lista ao final da lista.

python

    minha_lista = [1, 2, 3]

    # Usando append()
    minha_lista.append(4)
    print(minha_lista)  # Output: [1, 2, 3, 4]

    # Usando insert()
    minha_lista.insert(1, 1.5)
    print(minha_lista)  # Output: [1, 1.5, 2, 3, 4]

    # Usando extend()
    minha_lista.extend([5, 6])
    print(minha_lista)  # Output: [1, 1.5, 2, 3, 4, 5, 6]

Removendo Elementos

    remove(): Remove a primeira ocorrência de um elemento.
    pop(): Remove um elemento pelo índice e o retorna.
    clear(): Remove todos os elementos da lista.

python

minha_lista = [1, 2, 3, 4, 5, 2]

    # Usando remove()
    minha_lista.remove(2)
    print(minha_lista)  # Output: [1, 3, 4, 5, 2]

    # Usando pop()
    elemento = minha_lista.pop(3)
    print(minha_lista)  # Output: [1, 3, 4, 2]
    print(elemento)  # Output: 5

    # Usando clear()
    minha_lista.clear()
    print(minha_lista)  # Output: []

Funções e Métodos Úteis

    len(): Retorna o número de elementos na lista.
    sorted(): Retorna uma nova lista ordenada.
    sort(): Ordena a lista in-place.
    reverse(): Inverte a ordem dos elementos in-place.
    index(): Retorna o índice da primeira ocorrência de um valor.
    count(): Retorna o número de ocorrências de um valor.

python

    minha_lista = [3, 1, 4, 1, 5, 9, 2, 6, 5]

    # Usando len()
    print(len(minha_lista))  # Output: 9

    # Usando sorted()
    print(sorted(minha_lista))  # Output: [1, 1, 2, 3, 4, 5, 5, 6, 9]

    # Usando sort()
    minha_lista.sort()
    print(minha_lista)  # Output: [1, 1, 2, 3, 4, 5, 5, 6, 9]

    # Usando reverse()
    minha_lista.reverse()
    print(minha_lista)  # Output: [9, 6, 5, 5, 4, 3, 2, 1, 1]

    # Usando index()
    print(minha_lista.index(5))  # Output: 2

    # Usando count()
    print(minha_lista.count(1))  # Output: 2

List Comprehensions

List comprehensions são uma maneira concisa de criar listas.

python

    # Criando uma lista de quadrados
    quadrados = [x**2 for x in range(10)]
    print(quadrados)  # Output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

    # Criando uma lista de números pares
    pares = [x for x in range(10) if x % 2 == 0]
    print(pares)  # Output: [0, 2, 4, 6, 8]

Listas Aninhadas

Listas podem conter outras listas, permitindo a criação de estruturas complexas como matrizes.

python

    matriz = [
        [1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]
    ]

    # Acessando um elemento na matriz
    print(matriz[1][2])  # Output: 6

    # Iterando sobre uma matriz
    for linha in matriz:
        for elemento in linha:
            print(elemento, end=' ')
        print()

Esses são os fundamentos das listas em Python. Com essas informações, você pode começar a utilizar listas de maneira eficaz em seus programas.