Conjuntos em Python são coleções de elementos únicos e não ordenados. Eles são muito úteis quando você precisa garantir que todos os elementos sejam distintos ou quando você precisa realizar operações matemáticas de conjunto, como união, interseção e diferença. Aqui está uma visão geral de como trabalhar com conjuntos em Python:
Criando Conjuntos

Você pode criar um conjunto utilizando a função set() ou usando chaves {}. Para um conjunto vazio, você deve usar set() e não {}, pois {} cria um dicionário vazio.

python

    # Criando um conjunto com elementos
    conjunto = {1, 2, 3, 4, 5}
    print(conjunto)

    # Criando um conjunto vazio
    conjunto_vazio = set()
    print(conjunto_vazio)

Adicionando e Removendo Elementos

Para adicionar elementos a um conjunto, utilize o método add(). Para remover, use remove() ou discard().

python

    # Adicionando elementos
    conjunto.add(6)
    print(conjunto)

    # Removendo elementos
    conjunto.remove(3)  # Gera erro se o elemento não existir
    print(conjunto)

    conjunto.discard(2)  # Não gera erro se o elemento não existir
    print(conjunto)

Operações de Conjunto
União

A união de dois conjuntos contém todos os elementos de ambos os conjuntos. Use o operador | ou o método union().

python

    A = {1, 2, 3}
    B = {3, 4, 5}

    # Usando o operador |
    uniao = A | B
    print(uniao)

    # Usando o método union()
    uniao = A.union(B)
    print(uniao)

Interseção

A interseção de dois conjuntos contém apenas os elementos presentes em ambos. Use o operador & ou o método intersection().

python

    intersecao = A & B
    print(intersecao)

    intersecao = A.intersection(B)
    print(intersecao)

Diferença

A diferença entre dois conjuntos contém os elementos que estão no primeiro conjunto, mas não no segundo. Use o operador - ou o método difference().

python

    diferenca = A - B
    print(diferenca)

    diferenca = A.difference(B)
    print(diferenca)

Diferença Simétrica

A diferença simétrica entre dois conjuntos contém os elementos que estão em um dos conjuntos, mas não em ambos. Use o operador ^ ou o método symmetric_difference().

python

    dif_simetrica = A ^ B
    print(dif_simetrica)

    dif_simetrica = A.symmetric_difference(B)
    print(dif_simetrica)

Verificando Subconjuntos e Superconjuntos

Para verificar se um conjunto é subconjunto ou superconjunto de outro, use os métodos issubset() e issuperset().

python

    C = {1, 2}

    # Verificando se C é subconjunto de A
    print(C.issubset(A))

    # Verificando se A é superconjunto de C
    print(A.issuperset(C))

Iterando sobre Conjuntos

Você pode iterar sobre um conjunto usando um loop for.

python

    for elemento in A:
        print(elemento)

Compreensão de Conjuntos

Assim como listas e dicionários, você pode usar compreensão de conjuntos para criar um conjunto de maneira concisa.

python

    quadrados = {x ** 2 for x in range(10)}
    print(quadrados)

Conjuntos em Python são uma ferramenta poderosa para trabalhar com coleções de elementos únicos e realizar operações matemáticas de conjunto de forma eficiente e intuitiva.
