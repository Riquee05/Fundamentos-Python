Um dicionário em Python é uma coleção de pares chave-valor, onde cada chave é única dentro do dicionário. Eles são mutáveis e altamente eficientes para armazenar e acessar dados. Aqui estão algumas operações básicas que você pode realizar com dicionários em Python:
Criando um Dicionário

Você pode criar um dicionário usando chaves {} ou a função dict().

python

    # Usando chaves
    meu_dicionario = {
        'nome': 'João',
        'idade': 25,
        'cidade': 'São Paulo'
    }

    # Usando a função dict
    meu_dicionario2 = dict(nome='Maria', idade=30, cidade='Rio de Janeiro')

Acessando Valores

Você pode acessar os valores de um dicionário usando as chaves.

python

    nome = meu_dicionario['nome']  # 'João'
    idade = meu_dicionario['idade']  # 25

    Para evitar um erro se a chave não existir, você pode usar o método get.

python

    profissao = meu_dicionario.get('profissao', 'Desconhecido')  # 'Desconhecido'

Adicionando ou Atualizando Itens

Você pode adicionar um novo par chave-valor ou atualizar um valor existente.

python

    meu_dicionario['profissao'] = 'Engenheiro'
    meu_dicionario['idade'] = 26  # Atualiza a idade

Removendo Itens

Você pode remover itens usando del ou o método pop.

python

    del meu_dicionario['cidade']  # Remove a chave 'cidade'

    idade = meu_dicionario.pop('idade')  # Remove e retorna o valor associado à chave 'idade'

Iterando sobre um Dicionário

Você pode iterar sobre as chaves, valores ou pares chave-valor de um dicionário.

python

    # Iterando sobre as chaves
    for chave in meu_dicionario:
        print(chave, meu_dicionario[chave])

    # Iterando sobre os valores
    for valor in meu_dicionario.values():
        print(valor)

    # Iterando sobre os pares chave-valor
    for chave, valor in meu_dicionario.items():
        print(chave, valor)

Métodos Úteis

Existem vários métodos úteis para dicionários em Python:

    keys(): Retorna uma visão das chaves.
    values(): Retorna uma visão dos valores.
    items(): Retorna uma visão dos pares chave-valor.
    clear(): Remove todos os itens do dicionário.
    update(): Atualiza o dicionário com pares chave-valor de outro dicionário ou iterável.

python

    chaves = meu_dicionario.keys()  # Retorna as chaves
    valores = meu_dicionario.values()  # Retorna os valores
    itens = meu_dicionario.items()  # Retorna os pares chave-valor

    meu_dicionario.update({'pais': 'Brasil', 'idade': 27})  # Atualiza ou adiciona novas chaves
    meu_dicionario.clear()  # Limpa o dicionário

Exemplo Completo

Aqui está um exemplo completo que demonstra a criação, atualização, e iteração sobre um dicionário.

python

    # Criando um dicionário
    contatos = {
        'Alice': 'alice@example.com',
        'Bob': 'bob@example.com',
        'Eve': 'eve@example.com'
    }

    # Adicionando um novo contato
    contatos['Charlie'] = 'charlie@example.com'

    # Atualizando o e-mail de um contato existente
    contatos['Eve'] = 'eve_new@example.com'

    # Iterando sobre os contatos
    for nome, email in contatos.items():
        print(f'Nome: {nome}, E-mail: {email}')

    # Removendo um contato
    del contatos['Bob']

    # Verificando se uma chave existe no dicionário
    if 'Alice' in contatos:
        print('Alice está na lista de contatos')

    # Usando o método get para evitar erros de chave
    email = contatos.get('Daniel', 'Não encontrado')
    print(f'E-mail de Daniel: {email}')

Os dicionários são uma parte fundamental da programação em Python devido à sua flexibilidade e eficiência em operações de busca, inserção e exclusão.
