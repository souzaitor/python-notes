# Python Notes

Cheatsheet básica de Python baseada em estudos do livro Learning Python: Powerful Object‑Oriented, de Mark A. Lutz, e outras referências

## Sumário

- [Introdução](#introdução)
  - [Operadores Matemáticos](#operadores-matemáticos)
  - [Conversão de Dados](#conversão-de-dados)
  - [Variáveis](#variáveis)
  - [Comentários](#comentários)
  - [Docstrings](#docstrings)
  - [Função print()](#função-print)
  - [Função input()](#função-input)
- [Listas](#listas)
  - [Incializando Listas](#incializando-listas)
  - [Indexação e Slicing de Listas](#indexação-e-slicing-de-listas)
  - [Concatenação e Replicação de Listas](#concatenação-e-replicação-de-listas)
  - [Testando Existência em Listas](#testando-existência-em-listas)
  - [Adicionando Valores em Listas](#adicionando-valores-em-listas)
  - [Removendo Valores de Listas](#removendo-valores-de-listas)
  - [Ordenando Listas](#ordenando-listas)
  - [Encontrando Valores em Listas](#encontrando-valores-em-listas)
- [Tuplas](#tuplas)
  - [Inicializando Tuplas](#inicializando-tuplas)
  - [Indexação e Slicing de Tuplas](#indexação-e-slicing-de-tuplas)
  - [Alterando Tuplas](#alterando-tuplas)
  - [Deletando Tuplas](#deletando-tuplas)
  - [Testando Existência em Tuplas](#testando-existência-em-tuplas)
  - [Métodos de Tuplas](#métodos-de-tuplas)
- [Conjuntos](#conjuntos)
  - [Inicializando Conjuntos](#inicializando-conjuntos)
  - [Adicionando Elementos em Conjuntos](#adicionando-elementos-em-conjuntos)
  - [Removendo Elementos de Conjuntos](#removendo-elementos-de-conjuntos)
  - [Operaçõs de Teoria dos Conjuntos](#operas-de-teoria-dos-conjuntos)
  - [Testando Existência em Conjuntos](#testando-existência-em-conjuntos)
- [Dicionários](#dicionários)
  - [Inicializando Dicionários](#inicializando-dicionários)
  - [Inserindo Elementos em Dicionários](#inserindo-elementos-em-dicionários)
  - [Alterando Elementos de Dicionários](#alterando-elementos-de-dicionários)
  - [Removendo Elementos de Dicionários](#removendo-elementos-de-dicionários)
  - [Métodos keys(), values() e items()](#métodos-keys-values-e-items)
  - [Outros Métodos de Dicionários](#outros-métodos-de-dicionários)
  - [Testando Existência em Dicionários](#testando-existência-em-dicionários)
- [Strings](#strings)
  - [Instanciando Strings](#instanciando-strings)
  - [Deletando Strings](#deletando-strings)
  - [Indexação e Slicing em Strings](#indexação-e-slicing-em-strings)
  - [Testando Existência em Strings](#testando-existência-em-strings)
  - [Métodos startswith() e endswith()](#métodos-startswith-e-endswith)
  - [Métodos join() e split()](#métodos-join-e-split)
  - [Métodos isX](#métodos-isx)
  - [Capitalizando Strings](#capitalizando-strings)
  - [Removendo Espaços em Branco](#removendo-espaços-em-branco)
  - [Justificando Strings](#justificando-strings)
- [Formatação de Strings](#formatação-de-strings)
  - [Operador %](#operador-)
  - [Códigos de Formatação de Strings](#códigos-de-formatação-de-strings)
  - [Método str.format](#método-strformat)
- [Declarações Condicionais](#declarações-condicionais)
  - [Declaração if](#declaração-if)
  - [Declaração else](#declaração-else)
  - [Declaração elif](#declaração-elif)
  - [Testes](#testes)
  - [Operador Condicional Ternário](#operador-condicional-ternário)
- [Declarações de Repetição](#declarações-de-repetição)
  - [Declaração while](#declaração-while)
  - [Declaração break](#declaração-break)
  - [Declaração continue](#declaração-continue)
  - [Declaração for](#declaração-for)
  - [Declaração for com range()](#declaração-for-com-range)
  - [Declaração for com enumerate()](#declaração-for-com-enumerate)
  - [Declaração for else](#declaração-for-else)
  - [Declaração for com zip()](#declaração-for-com-zip)
- [Funções](#funções)
  - [Definição e Chamada de Função](#definição-e-chamada-de-função)
  - [Declaração return](#declaração-return)
  - [Argumentos Padrão](#argumentos-padrão)
  - [Argumentos Posicionais](#argumentos-posicionais)
  - [Argumentos Nominais](#argumentos-nominais)
  - [Argumentos Arbitrários](#argumentos-arbitrários)
- [Funções Lambda](#funções-lambda)
- [Escopo](#escopo)
  - [Escopo Local e Global](#escopo-local-e-global)
  - [Declaração global](#declaração-global)
  - [Declaração nonlocal](#declaração-nonlocal)
- [Arquivos](#arquivos)
  - [Abrindo arquivos](#abrindo-arquivos)
  - [Fechando Arquivos](#fechando-arquivos)
  - [Escrevendo em Arquivos](#escrevendo-em-arquivos)
  - [Lendo Arquivos](#lendo-arquivos)
  - [Métodos de Arquivos](#métodos-de-arquivos)
- [Módulos](#módulos)
  - [Importando Módulos](#importando-módulos)
- [Tratamento de Exceções](#tratamento-de-exceções)

## Introdução 

### Operadores Matemáticos

Em ordem de **precedência**:

| Operadores | Operação | Exemplo |
| -------- | -------- | -------- |
|** |Exponenciação| 2 ** 3 = 8|
|%| Módulo / Resto| 22 % 8 = 6|
|// |Divisão Inteira |22 // 8 = 2|
|/ |Divisão |22/8 = 2,75|
|* |Multiplicação| 3 * 3 = 9|
|- |Subtração| 5 - 2 = 3|
|+ |Adição |2 + 2 = 4|

### Conversão de Dados

```python
# Inteiro para String
>>> str(50)
'50'

# Inteiro para Float
>>> str(3.14)
'3.14'

# Float para Inteiro
>>> int(3.14)
3
```

### Variáveis

Regras:
* Deve ser apenas uma palavra.
* Deve usar apenas letras, números e o caractere sublinhado (_).
* Não pode começar com um número.
* Os nomes das variáveis que começam com um sublinhado (_) são considerados "inúteis"

### Comentários

```python
# Isso é um comentário
```

### Docstrings

Docstrings são strings usadas como documentação logo após a definição de uma função, método, classe ou módulo. Podemos acessar essas docstrings usando o atributo __doc__.

```python
>>> def func():
>>>   """
>>>   Isso é uma docstring
>>>   Também pode-se usar:
>>>   ''' Docstring '''
>>>   """
>>>
>>> print(func.__doc__)
Isso é uma docstring
Também pode se usar:
''' Docstring '''
```
### Função print()

```python
print([object, ...][, sep=' '][, end='\n'][, file=sys.stdout])
```

Argumentos entre colchetes são opcionais e podem ser omitidos em uma chamada, se omitidos os valores default são usados, esta função imprime a representação textual de um ou mais objetos separados pela string **sep** e seguido pelo **end** da string para o fluxo **file**.

```python
x = 'Olá' 
y = 39
z = ['Mundo']

>>> print(x, y, z)
Olá 39 ['Mundo']

# Sem pular linha
>>> print(x, y, z, end='')                        
Olá 39 ['Mundo']>>>

# Fim de linha personalizado
>>> print(x, y, z, end='...\n')
Olá 39 ['Mundo']...

# Separador personalizado
>>> print(x, y, z, sep='...')
Olá...39...['Mundo']
```
### Função input()
Lê uma string do teclado:

```python
>>> num = input('Entre com um número: ')
Entre com um número: 10
>>> num
'10'
```
[Voltar ao Topo](#sumário)


## Listas

> Listas são a coleção ordenada de objetos mais flexível. Podem conter qualquer tipo de objetos e podem ser alteradas localmente por atribuição,  chamadas de métodos, etc - são objetos mutáveis.

### Incializando Listas

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L
['gato', 'cachorro', 'rato', 'boi']
```

### Indexação e Slicing de Listas

O slicing gera sublistas que podem ser armazenados em uma nova lista.
Os valores acessados por indexão poder ser usados para alterar a lista

```python
# Indexação
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L[0] 
'gato'
>>> L[-1] 
'boi'

# Slicing
>>> L[1:3] 
['cachorro', 'rato']
>>> L[0:-1] 
['gato', 'cachorro', 'rato']
>>> L[:2] 
['gato', 'cachorro']
>>> L[1:] 
['cachorro', 'rato', 'boi']

# Alerar lista por indexação
>>> L
['gato', 'cachorro', 'rato', 'boi']
>>> L[0] = 'aushaus'
>>> L
['aushaus', 'cachorro', 'rato', 'boi']
```

### Concatenação e Replicação de Listas

```python
>>> [1, 2, 3] + ['A', 'B', 'C']
[1, 2, 3, 'A', 'B', 'C']

>>> ['X', 'Y', 'Z'] * 3
['X', 'Y', 'Z', 'X', 'Y', 'Z', 'X', 'Y', 'Z']

>>> L = [1, 2, 3]
>>> L = L + ['A', 'B', 'C']
>>> L
[1, 2, 3, 'A', 'B', 'C']
```

### Testando Existência em Listas

Podemos testar se um elemento existe ou não em uma lista usando **in**.

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> 'boi' in L
True
>>> 'gado' in L
False
```

### Adicionando Valores em Listas

**append()** adiciona um elemento ao final da lista:

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.append('cobra')
>>> L
['gato', 'cachorro', 'rato', 'boi', 'cobra']
```

**insert()** adiciona um elemnto na posição desejada:

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.insert(0, 'cobra')
>>> L
[ 'cobra', 'gato', 'cachorro', 'rato', 'boi']
```

**extend()** adiciona todos os elementos de um iterável (lista, tupla, string etc.) ao final da lista:

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.extend(['sapo', 'urso'])
>>> L
['gato', 'cachorro', 'rato', 'boi', 'sapo', 'urso']
```

### Removendo Valores de Listas

**remove()** remove o primeiro elemento correspondente da lista, só o primeiro será removido:

```python
>>> L = ['cobra', 'gato', 'gato']
>>> L.remove('gato')
>>> L
['cobra', 'gato']
```

**del** remove o item em um índice específico:

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> del L[0]
>>> L
['cachorro', 'rato', 'boi']
```

**pop()** remove o item em um índice específico e o retorna.

```python
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.pop (0)
'gato'
>>> L
['cachorro', 'rato', 'boi']
```

### Ordenando Listas

**sort()** ordena os elementos de uma lista em uma ordem crescente ou decrescente específica

```python
# Ordem crescente
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.sort()
>>> L
['boi', 'cachorro', 'gato', 'rato']

# Ordem decrescente
>>> L = ['gato', 'cachorro', 'rato', 'boi']
>>> L.sort(reverse=True)
>>> L
['rato', 'gato', 'cachorro', 'boi']

# Ordem crescente da função len()
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> L.sort(key=len)
>>> L
['boi', 'rato', 'gaviao', 'cachorro']
```

O método **sorted()** pode ser usado da mesma maneira mas retornaando a lista ordenada, passando a lista a ser ordenada como parâmetro:

```python
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> sorted(L)
['boi', 'cachorro', 'gaviao', 'rato']
```

O método **reverse()** inverte a ordem da lista:

```python
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> L.reverse()
>>> L
['boi', 'rato', 'cachorro', 'gaviao']
```

### Encontrando Valores em Listas

**index()** retorna o índice do elemento especificado na lista:

```python=
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> L.index('gaviao')
0
```

**len()** retorna a quantidade de elementos da lista ou comprimento: 

```python
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> len(L)
4
```

**count()** retorna o número de vezes que o elemento especificado aparece na lista.


```python
>>> L = ['gaviao', 'cachorro', 'rato', 'boi']
>>> L.count('rato')
1
```
[Voltar ao Topo](#sumário)

## Tuplas

> Tuplas formar grupos de objetos de forma simples. Funcionam exatamente como listas, exceto que tuplas não podem ser alteradas localmente (são imutáveis) e geralmente são escritos como uma série de itens entre parênteses, não colchetes.

### Inicializando Tuplas

Uma tupla pode ter qualquer número de itens e eles podem ser de tipos diferentes (inteiro, float, lista, string, etc.).

```python
# Tupla vazia
>>> T = ()

# Tupla com 1 elemento
>>> T = (1, )

# Tupla com elementos mistos
>>> T = (1, 'sapo', 3.4)
```

Uma tupla também pode ser criada sem o uso de parênteses. Isso é conhecido como empacotamento de tupla. Desempacotamento também é possível:

```python
# Empacotamento
>>> T = 3, 4, 'sapo'
>>> T
(3, 4, 'sapo')

# Desempacotamento
>>> a, b, c = T
>>> print(a, b, c)
3 4 5
```

### Indexação e Slicing de Tuplas

Podemos usar o operador de índice [] para acessar o elemento de uma tupla:

```python
# Indexação
>>> T = (3, 4, 'sapo')
>>> T[0]
3
>>> T[-1]
'sapo'
>>> T = (3, 4, (1, 2))
>> T[2][0]
(1, )

# Slicing
>>> T = (3, 4, 'sapo')
>>> T[:1]
(3,)
>>> T[1:]
(4, 'sapo')
>>> T[:-1]
(3, 4)
```

### Alterando Tuplas

Os elementos de uma tupla não podem ser alterados depois de atribuídos. Mas, se o próprio elemento for um tipo de dados mutável, como uma lista, seus itens aninhados podem ser alterados.

```python
>>> T = (4, 2, 3, [6, 5])

>>> T[1] = 9
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment

>>> T[3][0] = 9
>>> T
(4, 2, 3, [9, 5])
```

### Deletando Tuplas

Não podemos remover itens de uma tupla. A exclusão de uma tupla inteira usa **del**:

```python
>>> T = (1, 2, 3)
>>> T
(1, 2, 3)
>>> del T
```

### Testando Existência em Tuplas

Podemos testar se um elemento existe ou não em uma tupla usando **in**.

```python
>>> T = (1, 2, 3, 'boi')
>>> 'boi' in T
True
>>> 'gado' in T
False
```

### Métodos de Tuplas

**count()** retorna o número de vezes que o elemento especificado aparece na tupla:

```python
>>> T = (1, 1, 2, 3)
>>> T.count(1)
2
```

**index()** retorna o índice do elemento especificado na tupla:

```python
>>> T = (1, 2, 3)
>>> T.index(2)
2
```
[Voltar ao Topo](#sumário)

## Conjuntos

> Coleção não ordenada de objetos únicos e imutáveis, suportam operações matemáticas de teoria dos conjuntos. Por definição, um item aparece apenas uma vez em um conjunto, não importa quantos vezes é adicionado. 

### Inicializando Conjuntos

```python
>>> s = {1, 2, 3, 4}
>>> s = set([1, 2, 3, 4])
```

Ao criar um conjunto vazio, utilize a função **set()** ou você obterá um dicionário vazio.

```python
>>> s = {}
>>> type(s)
<class 'dict'>
```

O conjunto remove automaticamente todos os valores duplicados.

```python
>>> s = {1, 2, 3, 2, 3, 4}
>>> s
{1, 2, 3, 4}
```

E como um tipo de dados não ordenado, conjuntos não podem ser indexados.

```python
>>> s = {1, 2, 3}
>>> s [0]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'set' object does not support indexing
>>>
```

### Adicionando Elementos em Conjuntos

O método **add()** permite adicionar um único elemento ao conjunto.

```python
>>> s = {1, 2, 3, 4}
>>> s.add(5)
>>> s
{1, 2, 3, 4, 5}
```

O método **update()** permite adicionar vários elementos ao conjunto.

```python
>>> s = {1, 2, 3, 4}
>>> s.update([1, 5, 6, 7])
>>> s
{1, 2, 3, 4, 5, 6, 7}
```

### Removendo Elementos de Conjuntos

O método **remove()** remove um elemento do conjunto mostrando um **key error** se o elemento não pertencer ao conjunto.

```python
>>> s = {1, 2, 3, 4}
>>> s.remove(3)
>>> s
{1, 2, 4}
>>> s.remove(3)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
KeyError: 3
```

O método **discard())** remove um elemento do conjunto mas não mostra nenhum erro.

```python
>>> s = {1, 2, 3, 4}
>>> s.discard(3)
>>> s
{1, 2, 4}
>>> s.discard(3)
>>>
```

### Operaçõs de Teoria dos Conjuntos

União: **union()** ou | cria um novo conjunto com os elementos de ambos os conjuntos.

```python
>>> s1 = {1, 2, 3}
>>> s2 = {3, 4, 5}
>>> s1.union(s2) 
{1, 2, 3, 4, 5}
>>> s = s1 | s2
>>> s
{1, 2, 3, 4, 5}
```

Interseção: **intersection()** ou & cria um novo conjunto contendo apenas os elementos que são comuns a todos eles.

```python=
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s3 = {3, 4, 5}
>>> s1.intersection(s2, s3)  # or 
{3}
>>> s = s1 & s2 & s3
{3}
```

Diferença de Conjuntos: **difference()** ou - retorna os elementos que são únicos ao primeiro conjunto. 

```python=
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s1.difference(s2)  # ou 's1 - s2'
{1}
>>> s2.difference(s1) # ou 's2 - s1'
{4}
```
Diferença Simétrica: **symmetric_difference()** ou ^ retorna os elementos comum a ambos com excessão da interseção

```python
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s1.symmetric_difference(s2)
{1, 4}
>>> s = s1 ^ s2
>>> s
{1, 4}
```

### Testando Existência em Conjuntos

Podemos testar se um elemento existe ou não em um conjunto usando **in**.

```python
s = {1, 2, 3, 4}
1 in s
True
5 in s
False
```
[Voltar ao Topo](#sumário)

## Dicionários

> Dicionários são uma coleção não ordenada de itens. Cada item de um dicionário possui um par chave / valor. Os dicionários são otimizados para recuperar valores quando a chave é conhecida

### Inicializando Dicionários

Criar um dicionário é colocar itens entre chaves {} separados por vírgulas. Um item possui uma chave e um valor correspondente que é expresso como um par **(chave:valor)**.

O método **dict()** pode ser usado também.

```python
# Dicionário vazio
D = {}

# Dicionário com chaves inteiras
D = {1: 'maçã', 2: 'bola'}

# Dicionário com chaves mistas
D = {'nome': 'João', 1: [2, 4, 3]}

# Dsando dict()
D = dict ({1: 'maçã', 2: 'bola'})

# Sequência tendo cada item como um par
D = dict ([(1, 'maçã'), (2, 'bola')])
```

### Inserindo Elementos em Dicionários

```python
>>> D = {'nome': 'Pedro', 'idade': 22}
>>> D['cidade'] = 'São Paulo'
>>> D
{'nome': 'Pedro', 'idade': 22, 'cidade': 'São Paulo'}
```

### Alterando Elementos de Dicionários

```python
>>> D = {'nome': 'Pedro', 'idade': 22}
>>> D['nome'] = 'Lucas'
>>> D
{'nome': 'Lucas', 'idade': 22}
```

### Removendo Elementos de Dicionários

Podemos remover um item específico de um dicionário usando o método **pop()**. Este método remove um item com a chave fornecida e retorna o valor:

```python
>>> quadrados = {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
>>> quadrados.pop(4)
16
```

**popitem()** pode ser usado para remover e retornar um par de itens arbitrários (chave, valor) do dicionário. Todos os itens podem ser removidos de uma vez, usando o método **clear ()**:

```python
>>> quadrados = {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
>>> quadrados.popitem()
(5, 25)

>>> quadrados.clear()
>>> quadrados
{}
```

Também podemos **del** para remover itens individuais ou o  dicionário inteiro.

```python
>>> quadrados = {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

>>> del quadrados[1]
>>> quadrados
{2: 4, 3: 9, 4: 16, 5: 25}

>>> del quadrados
>>> quadrados
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'quadrados' is not defined
```

### Métodos keys(), values() e items()

**values()** retorna uma lista com todos os valores do dicionário:

```python
>>> D = {'cor': 'vermelho', 'idade': 20}
>>> for v in D.values():
>>>     print(v)
vermelho
20
```

**keys()** retorna uma lista com todas as chaves do dicionário:

```python
>>> D = {'cor': 'vermelho', 'idade': 20}
>>> for k in D.keys():
>>>     print(k)
cor
idade
```

**items()** retorna uma lista de tuplas dos pares (chave, valor) do dicionário:

```python
>>> D = {'cor': 'vermelho', 'idade': 20}
>>> for i in D.items():
>>>     print(i)
('cor', 'vermelho')
('idade', 20)
```
### Outros Métodos de Dicionários

**get()** retorna o valor da chave especificada se a chave estiver no dicionário:

```python
>>> D = {'uvas': 5, 'laranjas': 3}
>>> D.get{'uvas', 0}
5
# Retorna o segundo argumento como default
>>> D.get{'peras', 0}
0
```

**setdefault()** retorna o valor de uma chave (se a chave estiver no dicionário). Caso contrário, insere uma chave com um valor default:

```python
D = {'nome': 'Phill'}

# Chave não está no dicionário
>>> D.setdefault('salario')
>>> D
{'nome': 'Phill', 'salario': None}


# Chave não esta no dicionário, valor default
>>> D.setdefault('idade', 22)
>>> D
{'nome': 'Phill', 'idade': 22, 'salario': None}

```

### Testando Existência em Dicionários
Podemos testar se um elemento existe ou não em um dicionário usando **in**.

```
>>> D = {'nome': 'Paulo', 'idade': 7}
>>> 'nome' in D.keys()
True
>>> 'Paulo' in spam.values()
True
```

[Voltar ao Topo](#sumário)

## Strings

> Uma coleção ordenada de caracteres usados para armazenar e representar informações baseadas em texto. São sequências imutáveis, têm uma ordem posicional da esquerda para a direita e não podem ser alteradas localmente

### Instanciando Strings

```python
>>> S = 'Olá'
>>> S
'Olá'

>>> S = "Olá"
>>> S
'Olá'

>>> S = '''Olá'''
>>> S
'Olá'

# Aspas triplas podem ter várias linhas
>>> S = '''Olá
...     Mundo'''
>>> S
'Olá\n\tMundo'
```
### Deletando Strings

Não podemos excluir ou remover caracteres de uma string. Mas deletar a string inteiramente é possível usando **del**:

```python
>>> del S
>>> S
...
NameError: name 'S' is not defined
```

### Indexação e Slicing em Strings

```python
>>> S = 'Hello world!'

# Indexação
>>> S[0]
'H'

>>> spam[3]
'l'

>>> spam[-1]
'!'

# Slicing
>>> spam[6:-1]
'world'

>>> spam[:-1]
'Hello world'

>>> spam[::-1]
'!dlrow olleH'
```

### Testando Existência em Strings

Podemos testar se uma strings está contida ou não em uma string usando **in**:

```python
>>> 'Hello' in 'Hello World'
True
>>> 'Oi' in 'Hello World'
False
```

### Métodos startswith() e endswith() 

```python
>>> 'Hello world!'.startswith('Hello')
True

>>> 'Hello world!'.endswith('world!')
True

>>> 'abc123'.startswith('abcdef')
False

>>> 'abc123'.endswith('12')
False

>>> 'Hello world!'.startswith('Hello world!')
True

>>> 'Hello world!'.endswith('Hello world!')
True
```

### Métodos join() e split() 

**join()** retorna uma string juntando todos os elementos de um iterável separados por um separador de string.:

```python
>>> ', '.join(['cats', 'rats', 'bats'])
'cats, rats, bats'

>>> ' '.join(['My', 'name', 'is', 'Simon'])
'My name is Simon'

>>> 'ABC'.join(['My', 'name', 'is', 'Simon'])
'MyABCnameABCisABCSimon'
```

**split(**) quebra uma string no separador especificado e retorna uma lista de strings: 


```python
>>> 'My name is Simon'.split()
['My', 'name', 'is', 'Simon']

>>> 'MyABCnameABCisABCSimon'.split('ABC')
['My', 'name', 'is', 'Simon']

>>> 'My name is Simon'.split('m')
['My na', 'e is Si', 'on']
```
### Métodos isX

* **isalpha()** retorna True se a string consiste apenas em letras e não está em branco.
*  **isalnum()** retorna True se a string consiste apenas em letras e números e não está em branco.
* **isdecimal()** retorna True se a string consiste apenas em caracteres numéricos e não está em branco.
* **isspace()** retorna True se a string consiste apenas em espaços, tabulações e novas linhas e não está em branco.
* **istitle()** retorna True se a string consistir apenas em palavras que começam com uma letra maiúscula seguida por apenas letras minúsculas.
* **islower()** retorna True se todos os alfabetos em uma string forem letras minúsculas.
* **isupper()** retorna True se todos os caracteres em uma string forem letras maiúsculas.

### Capitalizando Strings

**upper()** converte todos os caracteres minúsculos em uma string em caracteres maiúsculos e os retorna:

```python
>>> S = 'Hello world!'
>>> S = S.upper()
>>> S
'HELLO WORLD!'
```

**lower()** converte todos os caracteres maiúsculos em uma string em caracteres minúsculos e os retorna.

```python
>>> S = 'HELLO WORLD!'
>>> S = S.lower()
>>> S
'hello world!'
```

### Removendo Espaços em Branco

```python
>>> S = '    Hello World     '
>>> S.strip()
'Hello World'

>>> S.lstrip()
'Hello World '

>>> S.rstrip()
'    Hello World'

>>> S = 'SpamSpamBaconSpamEggsSpamSpam'
>>> S.strip('ampS')
'BaconSpamEggs'
```
### Justificando Strings

**rjutst()** justifica a string para a direita e **ljust()** justifica a string para esquerda: 

```python
>>> 'Hello'.rjust(20)
'               Hello'

>>> 'Hello'.ljust(20)
'Hello               '
```

Um segundo argumento opcional é um caractere de preenchimento diferente de um caractere de espaço:

```python
>>> 'Hello'.ljust(20, '*')
'Hello***************'

>>> 'Hello'.rjust(20, '*')
'***************Hello'
```

**center()** retorna uma string centralizada:

```python
>>> 'Hello'.center(20)
'       Hello       '

>>> 'Hello'.center(20, '=')
'=======Hello========'

```



[Voltar ao Topo](#sumário)

## Formatação de Strings

### Operador %

Para formatar srings:
1. À esquerda do operador %, forneça uma string de formatação contendo um ou mais alvos de conversão combinados, cada um começando com uma %
2. À direita do operador %, forneça o objeto (ou objetos, embutidos em uma tupla) que você deseja que o Python insira na string de formato=ação à esquerda no lugar dos operadores

```python
>>> nome = 'Heitor'
>>> 'Olá %s' % nome
"Olá Heitor"
```
### Códigos de Formatação de Strings
| Código | Significado | 
| -------- | -------- | 
| s     | String     | 
|c |Caracter|
|d |Decimal (inteiro)|
|i| Inteiro|
|o| Octal inteiro|
|x |Hexadecimal inteiro|
|X |x, mas maiúsculo |
|e| expoente ponto flutuante, minúsculo|
|E |e, but prints maiúsculo|
|f |Ponto flutante decimal|
|F| Ponto flutante decimal|
|g| Ponto flutante e ou f|
|G| Ponto flutante E ou F |

### Método str.format

```python
# Por posição
>>> S = '{0} e {1}' 
>>> S.format ('carro', 'vermelho')
'carro e vermelho'

# Por palavra chave
>>> S = '{veiculo} e {cor}' 
>>> S.format (veiculo = 'carro', cor = 'vermelho')
'carro e vermelho'

# Ambos
>>> S = '{0} e {cor}'
>>> S.format ('carro', cor='vermelho')
'carro e vermelho'
```

Os códigos de formatação também pode ser usados:

```python
# Inteiros
>>> print("O número é:{:d}".format(123))
O número é:123

# Floats
>>> print("O número é:{:f}".format(123.4567898))
O número é:123.4567898

# octal, binário e hexadecimal 
>>> print("bin: {0:b}, oct: {0:o}, hex: {0:x}".format(12))
bin: 1100, oct: 14, hex: c
```

E outros códigos para arrendondamentos, sinais e alinhamento:

```python
>>> # Arrendondamento
>>> "Um terço é: {0:.3f}".format(1/3)
'Um terço é: 0.333'

>>> # Alinhamento
>>> "|{:<10}|{:^10}|{:>10}|".format('carro','carro','carro')
'|carro     |  carro   |     carro|'

# Sinais
>>> "Positivo: {:+d} e Negativo: {:-d} ".format(2,-2)
'Positivo: +2 e Negativo: -2 '
```

[Voltar ao Topo](#sumário)

## Declarações Condicionais

### Declaração if

```python
nome = 'Heitor'
if name == 'Heitor':
    print('Olá, Heitor.')
```

### Declaração else

```python
nome = 'Lucas'
if nome == 'Heitor':
    print('Olá, Heitor.')
else:
    print('Olá , estranho.')
```

### Declaração elif 

```python
nome = 'Heitor'
idade = 5
if nome == 'Heitor':
    print('Olá, Heitor.')
elif idade < 13:
    print('Você não é o Heitor, criança!')
else:
    print('Você não é o Heitor nem uma criança!')
```

```python
if <test1>:               # Teste if
    <statements1>         
elif <test2>:             # Elif opcional
    <statements2>
else:                     # Else opcional
    <statements3>
```

### Testes 

> Usar os operadores **in** e **not in** para avaliações booleanas e não == ou !=.

• Qualquer número diferente de zero ou objeto não vazio é verdadeiro.
• Números zero, objetos vazios e None são considerados falsos.
• Comparações e testes de igualdade são aplicados recursivamente às estruturas de dados.
• Comparações e testes de igualdade retornam Verdadeiro ou Falso (versões personalizadas de 1 e 0).
• Os operadores booleanos e e ou retornam um objeto operando verdadeiro ou falso.

### Operador Condicional Ternário

> A = Y if X else Z

```python
>>> A = 'true' if 'spam' else 'false'  # Não vazio é True
>>> A
'true'
>>> A = 'true' if '' else 'false' # Vazio é False
>>> A
'false'
```

## Declarações de Repetição

### Declaração while

```python
count = 0
while count < 5:
    print(count)
    count = count + 1
```

### Declaração break

A declarações **break** causa uma saída imediata de um loop.

```python
while True:
    nome = input('Entre com um nome: ')
    if nome == 'Heitor':
        break
print('Fim!!')
```

### Declaração continue

A declaração **continue** causa um salto imediato para o início de um loop:

```python
while True:
    nome = input('Entre com um nome: ')
    if nome == 'Heitor':
        break
print('Fim!!')
```
### Declaração for 
Um loop for pode iterar por qualquer tipo de sequência:

```python
# Lista
>>> for x in ["pao", "ovos", "presunto"]:
...     print(x, end=' ')
...
pao ovos presunto

# String
>>> S = 'Python'
>>> for x in S:
...     print(x, end=' ')
...
P y t h o n

# Tupla
>>> T = ("Olá", "mundo", "!")
>>> for x in T: 
...    print(x, end=' ')  
...
Olá mundo !
```

### Declaração for com range()

**range()** retorna uma série numérica no intervalo enviado como argumento. É comum com a estrutura **for**, cada ciclo o próximo elemento da sequência será utilizado de tal forma que é possível partirmos de um ponto e ir incrementando, decrementando x unidades.

```python
>>> print('Meu nome é')
>>> for i in range(5):
>>>     print('Heitor Cinco Vezes ({})'.format(str(i)))
Meu nome é
Heitor Cinco Vezes (0)
Heitor Cinco Vezes (1)
Heitor Cinco Vezes (2)
Heitor Cinco Vezes (3)
Heitor Cinco Vezes (4)
```

**range()** também pode ser chamada com três argumentos. Os primeiros dois argumentos serão os valores inicial e final, e o terceiro será o argumento do passo. O passo é o valor pelo qual a variável é aumentada após cada iteração.


### Declaração for com enumerate()

**enumerate()** é usado para quando é necessãrio iterar pelo loop a posição e o valor do item de uma seqência ao mesmo tempo:

```python
>>> S = 'python'
>>> for for (pos, item) in enumerate(S)
...     print(item, 'posição', pos)
...
p posição 0
y posição 1
t posição 2
h posição 3
o posição 4
n posição 5
```

### Declaração for else 

Permite especificar uma instrução a ser executada no caso do loop completo ter sido executado. Útil apenas quando uma condição **break** pode ocorrer no loop:

```python
>>> for i in [1, 2, 3, 4, 5]:
>>>    if i == 3:
>>>        break
>>> else:
>>>    print("só executado quando nenhum item da lista for igual a 3")
```
### Declaração for com zip()

**zip()** recebe uma ou mais sequências como argumentos e retorna uma série de tuplas que emparelham itens paralelos tomados a partir dessas sequências:

```python
>>> nome = ['Lucas', 'Pedro', 'Ana']
>>> idade = [6, 23, 44]
>>> for n, i in zip(nome, idade):
>>>     print('{} tem {} anos'.format(n, i))
Lucas tem 6 anos
Pedro tem 23 anos
Ana tem 44 anos
```


[Voltar ao Topo](#sumário)
## Funções

> Função é um grupo de declarações relacionadas que executam uma tarefa específica.

### Definição e Chamada de Função

```python
# Definição
>>> def bomdia(nome):
>>>    print("Bom dia, " + nome + "!")
>>>

# Chamada
>>> bomdia("Heitor")
Bom dia, Heitor!
>>> bomdia("Ana")
Bom dia, Ana!
```

### Declaração return

**return** é usada para sair de uma função e voltar para o local de onde foi chamada, pode ser retornada uma expressão a ser avaliada ou **None** caso não haja expressão:

```python
# Retorna None
>>> def bomdia(nome):
>>>    print("Bom dia" + nome + "!")
>>> bomdia("Heitor")
Bom dia, Heitor!

# Retorna a string
>>> def bomdia(nome):
>>>    return "Bom dia, " + nome + "!"
bomdia("Heitor")
'Bom dia, Heitor!'

```

### Argumentos Padrão

Qualquer número de argumentos em uma função pode ter um valor padrão. Mas, uma vez que temos um argumento padrão, todos os argumentos à sua direita também devem ter valores padrão:


```python
>>> def bomdia(nome, msg = "Bom dia, "):
>>>    print(msg + nome + "!")
>>>
>>> bomdia("Heitor")
Bom dia, Heitor!
>>> bomdia("Heitor", "Boa tarde, ")
Boa tarde, Heitor!
```

### Argumentos Posicionais

A ordem dos argumentos é importante quando eles são passados posicionalmente:

```python
def bhaskara(a, b, c):
    x1 = -b / (2*a)
    x2 = sqrt(b**2 - 4*a*c) / (2*a)
    return (x1 + x2), (x1 - x2)

>>> bhaskara(31, 93, 62)
(-1.0, -2.0)

```

### Argumentos Nominais

ou **keyword/named arguments**, a ordem dos argumentos não importa quando eles são passados pelo nome:

```python
def bhaskara(a, b, c):
    x1 = -b / (2*a)
    x2 = sqrt(b**2 - 4*a*c) / (2*a)
    return (x1 + x2), (x1 - x2)	

>>> bhaskara(a=31, b=93, c=62)
(-1.0, -2.0)
>>> bhaskara(c=31, b=93, a=62)
(-0.5, -1.0)

```

### Argumentos Arbitrários

Na declaração de funções, * significa “empacotar todos os argumentos posicionais restantes em uma tupla chamada <nome>” e na chamada de funções significa “desempacotar tupla ou lista chamada <nome> para argumentos posicionais nesta posição”:


```python
>>> def frutas(*args):
>>>    for fruta in args:
>>>       print(fruta)

>>> fruits("macas", "bananas", "uvas")

"macas"
"bananas"
"uvas"

```
Na declaração de funções, ** significa o mesmo para argumentos de palavra-chave (exceto que usa um dicionário, não uma tupla) e na chamada de funções ** é o mesmo que *, só que para argumentos de palavra-chave:

```python
>>> def fruit(**kwargs):
>>>    for chave, valor in kwargs.items():
>>>        print("{0}: {1}".format(chave, valor))

>>> fruit(nome = "maca", cor = "vermelha")

nome: maca
cor: vermelha
```
## Funções Lambda

é uma função definida sem um nome. Enquanto as funções normais são definidas usando **def**, as funções anônimas são definidas usando **lambda**:

```python
>>> soma = x, y: x+y
>>> soma(2, 2)
4
```

Devem ser expressões de uma única linha

[Voltar ao Topo](#sumário)
## Escopo

### Escopo Local e Global

* O código no escopo global não pode usar nenhuma variável local.
* No entanto, um escopo local pode acessar variáveis globais.
* O código no escopo local de uma função não pode usar variáveis em qualquer outro escopo local.
* Você pode usar o mesmo nome para variáveis diferentes se elas estiverem em escopos diferentes.

### Declaração global

Usada se você precisa modificar uma variável global de dentro de uma função:

```python
>>> def func():
>>>     global a
>>>     a = 'local'
>>>
>>> a = 'global'
>>> func()
>>> a
'local'
```

### Declaração nonlocal

Usada quando a variável não pode estar no escopo local nem no global, em funções aninhadas:

```python
>>> def exter():
>>>    x = "local"
>>>    def externa():
>>>       nonlocal x
>>>       x = "nonlocal"
>>>       print("interna:", x)
>>>
>>>    inter()
>>>    print("externa:", x)
>>>
>>> outer()
interna: nonlocal
externa: nonlocal
```
[Voltar ao Topo](#sumário)

## Arquivos

### Abrindo arquivos

**open()** abre um arquivo e retorna um objeto arquivo, também chamado de handle. Podemos especificar o modo de abertura e o tipo do arquivo:


| Modo | Descrição | 
| -------- | -------- | 
| r     | Leitura (Padrão)     | 
| w | Gravação, cria um novo arquivo se ele não existir ou trunca o arquivo se ele existir |
| x | Criação exclusiva, se o arquivo já existir a operação falhará |
| a | Anexar no final do arquivo sem truncá-lo, cria um novo arquivo se ele não existir |
| t | Modo de texto | (Padrão) |
| b | Modo binário |
| + | Atualização (leitura e gravação) |


```python
>>> f = open ("test.txt") # Abrir arquivo no diretório atual
>>> f = open ("C: /Python/test.txt") # Especificando o diretório completo
>>> f = open ("test.txt", 'w') # Escrever em modo de texto
>>> f = open ("img.bmp", 'r + b') # Ler e escrever em modo binário
```

### Fechando Arquivos
Usando a função **close():**

```python
f = open("test.txt", encoding = 'utf-8')
# Operações de arquivo
f.close()
```

Usando a declaração **with** garantimos que o arquivo seja fechado quando o bloco for encerrado:

```python
with open("test.txt", encoding = 'utf-8') as f:
   # Operações de arquivo
```
### Escrevendo em Arquivos

Para escrever em um arquivo precisamos abri-lo no modo **w**, **a** ou **x**.  

A escrita de uma string ou sequência de bytes (para arquivos binários) é feita usando o método **write()**. Este método retorna o número de caracteres gravados no arquivo:

```python
with open("test.txt",'w',encoding = 'utf-8') as f:
   f.write("Meu primeiro arquivo\n")
   f.write("Esse arquivo\n")
   f.write("tem três linhas\n")
```

### Lendo Arquivos

Para ler um arquivo devemos abri-lo no modo **r**.

Podemos usar o método **read(tam)** para ler o número de tamanho dos dados. Se o parâmetro de tamanho não for especificado, ele lê e retorna até o final do arquivo:

```python
>>> f = open ("test.txt", 'r',encoding  = 'utf-8')
>>> f.read(4) # Lê os 4 primeiros dados
'Meu '

>>> f.read (4) # lê os próximos 4 dados
'prim'

>>> f.read () # Lê o resto até o final do arquivo
'eiro arquivo\nEsse arquivo\n\ntem três linhas\n'

>>> f.read () # Leitura adicional retorna string vazia
''
```

Podemos mudar nosso cursor de arquivo atual (posição) usando o método search (). Da mesma forma, o método tell () retorna nossa posição atual (em número de bytes):

```python
>>> f.tell() # Posição inicial
56
>>> f.seek(0) # Cursor na posição inicial
0
>>> print(f.read()) # Lê arquivo todo

Meu primeiro arquivo
Esse arquivo
tem três linhas
```

Podemos ler um arquivo linha por linha usando um **loop for**:

```python
>>> for line in f:
...     print(line, end = '')
Meu primeiro arquivo
Esse arquivo
tem três linhas
```

**readline()** lê as linhas individuais de um arquivo. Este método lê um arquivo até a nova linha, incluindo o caractere de nova linha (\n):

```python
>>> f = open("test.txt",'r',encoding = 'utf-8')
>>> f.readline()
'Meu primeiro arquivo\n'

>>> f.readline()
'Esse arquivo\n'

>>> f.readline()
'tem três linhas\n'

>>> f.readline()
''
```

**readlines()** retorna uma lista de linhas restantes de todo o arquivo:

```python
['Meu primeiro arquivo\n', 'Esse arquivo\n', '\n', 'tem três linhas\n']
```

Todos esses métodos de leitura retornam valores vazios quando o fim do arquivo (EOF) é atingido.

### Métodos de Arquivos

| Método | Descrição | 
| -------- | -------- | 
| close() | Fecha um arquivo aberto. Não tem efeito se o arquivo já estiver fechado |
| detach() | Separa o buffer binário subjacente da **TextIOBase** e o retorna |
| fileno() | Retorna um número inteiro (descritor de arquivo) do arquivo |
| flush | Libera o buffer de gravação do fluxo de arquivos |
| isatty() | Retorna isatty se o fluxo de arquivo for interativo |
| read(n) | Lê no máximo n caracteres do arquivo. Lê até o final do arquivo se for negativo ou None |
| readable() | Retorna **True** se o fluxo do arquivo pode ser lido |
| readline(n = -1) | Lê e retorna uma linha do arquivo. Lê no máximo n bytes, se especificado |
| readline(n = -1) | Lê e retorna uma lista de linhas do arquivo. Lê no máximo n bytes / caracteres, se especificado |
| seek(posicao, from = SEEK_SET) | Altera a posição do arquivo para bytes de posição, em referência a from(início, atual, fim) |
| seekable() | Retorna **True** se o fluxo de arquivo suportar acesso aleatório |
| tell() | Retorna a localização do arquivo atual |
| truncate(tamanho = None) | Redimensiona o fluxo de arquivo para bytes de tamanho. Se o tamanho não for especificado, é redimensionado para a localização atual |
| writable() | Retorna **True** se o fluxo de arquivo pode ser gravado |
| write(S) | Grava a string s no arquivo e retorna o número de caracteres gravados |
| writelines(linhas) | Grava uma lista de linhas no arquivo|

[Voltar ao Topo](#sumário)

## Módulos

> Módulos referem-se a um arquivo contendo instruções e definições Python. 
Um arquivo contendo código Python, por exemplo: example.py, é chamado de módulo e seu nome de módulo seria example.

### Importando Módulos

```python
# Exemplo de módulo python
# example.py

def soma(a, b):
   """Soma dois número e retorna"""
   return a + b
```

**import** é usado para importar nosso um módulo definido anteriormente. Usando o nome do módulo podemos acessar as funções usando o operador ponto ( . ) : 

```python
>>> import example
>>> example.soma(4, 6)
10
```

Podemos importar um módulo renomeando-o :

```python
>>> import math as m
>>> print ("O valor de pi é", m.pi)
O valor de pi é 3.141592653589793
```

Podemos importar nomes específicos de um módulo sem importar o módulo todo:

```python
>>> from math import pi
>>> pi
3.141592653589793
```

[Voltar ao Topo](#sumário)

## Tratamento de Exceções

```python
>>> def func(num):
>>>     try:
>>>         return 42 / num
>>>     except ZeroDivisionError as e:
>>>         print('Error: Invalid argument: {}'.format(e))
>>>
>>> print(func(2))
>>> print(func(12))
>>> print(func(0))
>>> print(func(1))
21.0
3.5
Error: Invalid argument: division by zero
None
42.0
```

[Voltar ao Topo](#sumário)


