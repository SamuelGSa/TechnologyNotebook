
## ``Collections.sort()``;
Usado para classificar os elementos presentes na lista especificada de Coleção em ordem crescente
___

## ``List<E>``
Uma coleção ordenada.  O usuário tem controle preciso sobre onde na lista cada elemento é inserido. 

A lista permite elemento duplicados.
___

## ``Set<E>``
Uma coleção que não contém elementos duplicados

___

## ``Map<K,V>``
um Objeto que mapeia chaves para valores. Um mapa nao pode conter chaves duplicadas; Cada chave pode mapear no máximo um valor.

**fruta** : cor
**pera** : amarela

Possivel implementarmos os conjuntos de dados por meio de duas interfaces:
- Map
- SortedMap(Ordena as chaves)

### Usando suas 3 classes para ser implementada: 
- ``HashMap()`` : Não realiza a ordenação dos elementos.
- ``LinkedHashMap()`` : Ordena os elementos contidos no map em ordem de inserção. Suporta o uso de valor e chaves nulos ("null")
- ``TreeMap()`` : Usa ordenação ascendente. Bastante usado na manipulação de dados hierárquicos e não tem suporte para uso de valores nulos("**null**")

[Sobre Integer](https://www.alura.com.br/artigos/diferenca-entre-int-e-integer-em-java)

```
Map<objeto_chave, objeto_valor> nome_do_mapa = new tipo_de_dado();
Map<String,Integer> AgendaTelefonica = new HasMap();
```
*a Interface Map não pode ser instanciavel, usamos a class HashMap() para manipular o conjunto.*
___

## Métodos da interface Map

- ``.size()`` : retorna o tamanho do map(numero de pares)
- ``.isEmpty()`` : retorna true caso algum par esteja vazio
- ``.containsKey()`` e ``.containsValue()`` : retorna true para os casos em que o elemento verificado esteja presente e false, caso não.
- ``.get()`` : retorna o valor contido na chave especificada
- ``.put()`` e ``.remove()`` : colocar e remover elementos. Não retorna valores.
___

- ``forEach()`` :usado para iterar os valores e chaves da interface
- ``replace()`` : substituir elementos
- ``merge()`` : mesclar diferentes maps

___
## Iteração com HashMap

Existem varias maneiras de iterar no HashMap, essas sao 5 delas

- Loop for-each
- por meio de EntrySet de HashMap usando iteradores.
- Expressões Lambda

- Usando um iterador para iterar por meio de um HashMap
- API Stream
