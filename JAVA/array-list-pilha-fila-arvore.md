Reunião Ozelo 04/10 

ArrayList usa internamente um array para guardar os elementos. 
Ponto positivo: Se voce precisar pegar o décimo quinto elemento, ele te devolve bem rápido.
Ponto Negativo: Quando voce inserir um novo elemento na primeira posição. Se há muitos elementos, isso vai demorar.

LinkedList utiliza a estrutura de dados chamada Lista Ligada. 
Ponto positivo: Ela é muito rápida para adicionar e remover elementos na cabeça da lista.
Ponto negativo: Lenta se voce precisa acessar um determinado elemento
___

[Estrutura De Dados](https://pt.wikipedia.org/wiki/Estrutura_de_dados)
Principais Estruturas de Dados (Clássicas)

- Array
- Lista
- Pilha
- Fila
- Arvore

## Array
Também chamado de arranjo ou vetor e matriz, variável indexada.

Estrutura de dados que armazena uma coleção de elementos de tal forma que cada um dos elementos possa ser identificados por, pelo menos um índica ou uma chave.

Elementos individuais sao acessados por sua posição no arranjo. A posição é dada por um índice(**subscrição**)

Podem ser considerados como as estruturas de dados mais simples. Tem a vantagem de que os seus elementos são acessíveis de forma mais rápida mas tem uma notável **limitação**: são de tamanho fixo, mas podem ser incrementados ou diminuídos com determinados algoritmos.

A forma de acessar os elementos é **direta**. Isso quer dizer que o elemento desejado obtém-se a partir do seu índice e não é preciso procura-lo elemento por elemento.

``String[] S = new String[5];``
___

## Lista

Ou sequencia, é uma estrutura de dados **abstrata** que implementa uma coleção ordenada de valores, onde o mesmo valor pode ocorrer mais de uma vez. Uma instância de uma lista é uma representação computacional do conceito matemático de uma sequencia finita, que é, uma tupla. Cada instância de um valor na lista normalmente é chamado de um **item**, **entrada** ou **elemento** da lista. Se o mesmo valor ocorrer várias vezes, cada ocorrência é considerada um item distinto.

- Lista estática : permitem apenas a verificação e enumeração dos valores.
- Lista Mutável ou Dinâmica : pode permitir que itens sejam inseridos, substituídos ou excluídos durante a existência da lista.

### Tipos de implementação de listas como estruturas de dados:

- Lista duplamente Ligadas (*Estrutura ligada que consiste de um conjunto de registros sequencialmente ligados chamados nós e é uma extensão da lista simplesmente ligada. Cada nó contem dois campos, chamados de links ou enlaces, que são referências para o nó anterior e para o nó posterior na sequência de nós*.)
- Lista FIFO (First in First Out)
- Lista LIFO (Last in First Out)

Tamanho da lista significa o número de elementos presentes na lista. Listas encadeadas tem a vantagem de ter um tamanho variável, novos itens podem ser adicionados, o que aumentando seu tamanho.

Cada elemento numa lista possui um índice, um número que identifica cada elemento da lista. Usando o índice de um elemento da lista é possível buscá-lo ou removê-lo

## Pilha

Ou stack, é um tipo abstrato de dado e estrutura de dado baseado no princípio **LIFO**,  caracterizando um empilhamento de dados.

Pilhas são fundamentalmente compostas por duas operações:
- **Push**(empilhar) que adiciona um elemento no tpo da pilha
- **Pop**(desempilhar) que remove o ultimo elemento adicionado.

Pilhas são usadas extensivamente em cad nível de um sistema de computação moderno.

Um pc moderno usa pilha ao nível de arquitetura, as quais sao usadas no design básico de um sistema operacional para manipular interrupções e chamadas de função do sistema operacional.

Usadas para executar uma JVM e a própria linguagem java possui uma classe denominada "Stack", as quais podem ser usadas.

## Fila
**FIFO**, é im algoritmo de escolamento para estruturas de dados do tipo fila.
É um algoritmo de escalonamento não preemptivo que entrega a CPU os processos pela ordem de chegada.
 
(No **escalonamento não-preemptivo**, quando um processo está em execução, nenhum evento externo pode ocasionar a perda do uso do processador. O processo somente sai do estado de execução, caso termine seu processamento ou execute instruções do próprio código que ocasionem uma mudança para o estado de espera.)

Ele executa o processo como um todo do inicio ao fim, não interrompendo o processo executado até ser finalizado, então quando u novo processo chega e existe um em execução, ele vai para uma fila de espera

Nesse escalonamento todos os processos tendem a serem atendidos (evitando o fenômeno de starvation/inanição) a menos que um processo possua erro ou loop infinito

Em programação concorrente, ocorre **inanição** quando um processo nunca é executado ("morre de fome"), pois processos de prioridade maior sempre o impedem de ser executado.

FIFO não garante um tempo de resposta rápido pois é extremamente sensível a ordem de chegada de cada processo e dos antecessores e se processos que tendem a demorar mais tempo chegarem primeiro o tempo médio de espera e o turnaround acaba sendo aumentados

## Arvore

Uma das mais importantes estruturas de dados nao lineares.
Nas árvores, os dados estão dispostos de forma hierárquica, seus elementos encontram "acima" ou "abaixo" de outros elementos da árvore

Estruturas eficientes e simples em relação ao tratamento computacional. Há inúmeros problemas no mundo real que podem ser modelados e resolvidos através das árvores. 

**Ex**: Estruturas de pastas de um SO, interfaces gráficas, banco de dados e sites da internet 

Formada por um conjunto de elementos que armazenam informações chamados **nodos** ou **nós**. Toda árvore possui o elemento chamado raiz, que possui ligações para outros elementos denominados amos ou filhos.

O elemento que não possui ramos é conhecido como **nó folha**, **nó terminal** ou **nó externo**.


____
garbage collector  -> JAVA

busca binária 


faça um programa simples em java

cria uma lista com random de 10k números
criar e um list de java
um map (qual a forma mais eficiente de iterar  em um hashmap)
e um set

Collections.sort();
Set;
List;
Map;





