Manipulação de strings em Python é uma tarefa comum e há diversas técnicas e métodos disponíveis para facilitar essa manipulação. A seguir, vou apresentar algumas operações básicas e avançadas para manipular strings em Python.
1. Criação e Básico de Strings

python

    # Criação de uma string
    minha_string = "Olá, Mundo!"

    # Imprimir a string
    print(minha_string)

2. Indexação e Fatiamento

python

    # Indexação (começa do 0)
    print(minha_string[0])  # 'O'
    print(minha_string[-1])  # '!'

    # Fatiamento (slice)
    print(minha_string[0:5])  # 'Olá, '
    print(minha_string[6:])  # 'Mundo!'
    print(minha_string[:5])  # 'Olá, '

3. Métodos de String Comuns

python

    # Conversão para maiúsculas e minúsculas
    print(minha_string.upper())  # 'OLÁ, MUNDO!'
    print(minha_string.lower())  # 'olá, mundo!'

    # Remover espaços em branco
    string_com_espacos = "  Olá, Mundo!  "
    print(string_com_espacos.strip())  # 'Olá, Mundo!'

    # Substituição de caracteres
    print(minha_string.replace("Mundo", "Python"))  # 'Olá, Python!'

    # Quebrar string em uma lista
    print(minha_string.split())  # ['Olá,', 'Mundo!']

    # Verificar se a string começa ou termina com algo
    print(minha_string.startswith("Olá"))  # True
    print(minha_string.endswith("!"))  # True

4. Formatação de Strings

4.1. Usando o operador %

python

    nome = "João"
    idade = 30
    print("Meu nome é %s e eu tenho %d anos." % (nome, idade))

4.2. Usando o método format

python

    print("Meu nome é {} e eu tenho {} anos.".format(nome, idade))
    print("Meu nome é {0} e eu tenho {1} anos.".format(nome, idade))
    print("Meu nome é {nome} e eu tenho {idade} anos.".format(nome=nome, idade=idade))

4.3. Usando f-strings (Python 3.6+)

python

    print(f"Meu nome é {nome} e eu tenho {idade} anos.")

5. Métodos Avançados

5.1. Juntar listas em uma string

python

    lista = ["Olá", "Mundo"]
    print(" ".join(lista))  # 'Olá Mundo'

5.2. Encontrar substrings

python

    print(minha_string.find("Mundo"))  # Retorna a posição inicial ou -1 se não encontrado
    print(minha_string.count("o"))  # Conta quantas vezes 'o' aparece na string

5.3. Alinhamento de Strings

python

    print(minha_string.center(20, '-'))  # '---Olá, Mundo!---'
    print(minha_string.ljust(20, '-'))  # 'Olá, Mundo!-------'
    print(minha_string.rjust(20, '-'))  # '-------Olá, Mundo!'

6. Expressões Regulares

Para manipulações mais complexas de strings, expressões regulares podem ser usadas com o módulo re.

python

import re

    # Encontrar todas as ocorrências de um padrão
    padrao = r'\b\w{3,}\b'  # Palavras com 3 ou mais letras
    texto = "Este é um exemplo com várias palavras"
    ocorrencias = re.findall(padrao, texto)
    print(ocorrencias)  # ['Este', 'exemplo', 'com', 'várias', 'palavras']

# Substituir ocorrências
    texto_modificado = re.sub(r'palavras', 'termos', texto)
    print(texto_modificado)  # 'Este é um exemplo com várias termos'

Estas são algumas das técnicas fundamentais e avançadas para manipulação de strings em Python. Cada método e técnica tem seu uso específico, dependendo do tipo de manipulação que você precisa realizar.