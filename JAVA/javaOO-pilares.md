# Java OO: Entendendo a Orientação a Objetos

*Programação orientada a objetos é um Paradigma de programação (forma de se programar)*

- É baseado sobre dois conceitos chaves: Classes e Objetos. 

Uma classe é um conjunto de características e comportamentos que definem o conjunto de objetos pertencentes à essa classe. Repare que a classe em si é um conceito abstrato, como um molde, que se torna concreto e palpável através da criação de um objeto. Chamamos essa criação de instanciação da classe, como se estivéssemos usando esse molde (classe) para criar um objeto.

**Exemplo: Carro**
- O seu carro tem as características que você estava procurando
- Ele também possui comportamentos que, provavelmente, foram o motivo de sua compra, como acelerar, acender os faróis,etc
- o carro novo é um objeto, onde suas características são seus atributos (dados atrelados ao objeto) e seus comportamentos são ações ou métodos
- Seu carro é um objeto seu, mas na loja onde você o comprou existiam vários outros, muito similares
Seu objeto pode ser classificado (isto é, seu objeto pertence à uma classe) como um carro, e que seu carro nada mais é que uma instância dessa classe chamada "carro".
___

## Pilares da OO - Encapsulamento

O encapsulamento de atributos e métodos impede o chamado **vazamento de escopo**, onde um atributo ou método é visível por alguém que não deveria vê-lo, como outro objeto ou classe. 
Isso evita a confusão do uso de variáveis globais no programa, deixando mais fácil de identificar em qual estado cada variável vai estar a cada momento do programa, já que a restrição de acesso nos permite identificar quem consegue modificá-la.

Um carro, por **exemplo** tem os métodos de acelerar e outro de injeção de combustível. Ao acelerar, você gasta combustível.
No entanto, se alguns desses atributos ou métodos forem facilmente visíveis e modificáveis, como o mecanismo de aceleração do carro, isso pode dar liberdade para que alterações sejam feitas, resultando em efeitos colaterais imprevisíveis. Nessa analogia, uma pessoa pode não estar satisfeita com a aceleração do carro e modifica a forma como ela ocorre, criando efeitos colaterais que podem fazer o carro nem andar.

Mas então, como sabemos como o nosso carro acelera? É simples: **não sabemos**. Nós só sabemos que para acelerar, devemos pisar no acelerador e de resto o objeto sabe como executar essa ação sem expor como o faz. 
Dizemos que a **aceleração do carro está encapsulada**, pois sabemos o que ele vai fazer ao executarmos esse método, mas não sabemos como - e na verdade, não importa para o programa como o objeto o faz, só que ele o faça.
O mesmo vale para atributos.
___

## Pilares da OO - Herança 

No caso do carro, dizemos então que um Honda Fit "Cross" é um tipo de Honda Fit, e o que muda são alguns atributos (paralama reforçado, altura da suspensão etc), e um dos métodos da classe (acelerar, pois agora há tração nas quatro rodas), mas todo o resto permanece o mesmo, e o novo modelo recebe os mesmos atributos e métodos do modelo clássico.

            ANIMAIS
    MAMIFERO        AVE
    Cachorro        Beija-Flor

Quando dizemos que uma classe A é um tipo de classe B, dizemos que a classe A herda as características da classe B e que a classe B é mãe da classe A, estabelecendo então uma relação de **herança** entre elas. No caso do carro, dizemos então que um Honda Fit "Cross" é um tipo de Honda Fit, e o que muda são alguns atributos (paralama reforçado, altura da suspensão etc), e um dos métodos da classe (acelerar, pois agora há tração nas quatro rodas), mas todo o resto permanece o mesmo, e o novo modelo recebe os mesmos atributos e métodos do modelo clássico.
___

## Pilares da OO - Interface 

Quando duas (ou mais) classes possuem comportamentos comuns que podem ser separados em uma outra classe, dizemos que a "classe comum" é uma interface, que pode ser "herdada" pelas outras classes. 
Uma interface não é exatamente um classe, mas sim um conjunto de métodos que todas as classes que herdarem dela devem possuir (**implementar**) - portanto, uma interface não é "herdada" por uma classe, mas sim implementada
___

## Pilares da OO - Polimorfismo

 Dizemos que o método "tocar música"(no exemplo dos carros terem sons diferentes) é uma forma de **polimorfismo**, pois dois objetos, de duas classes diferentes, têm um mesmo método que é implementado de formas diferentes, ou seja, um método possui várias formas, várias implementações diferentes em classes diferentes, mas que possuem o mesmo efeito ("polimorfismo" vem do *grego poli = muitas, morphos = forma*).
