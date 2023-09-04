# KAFKA
[Site do Kafka](https://kafka.apache.org/)

Apache kafka é uma plataforma de streaming de eventos distribuída, Open Source, usada para **pipelines** de dados de alto desempenho, análise de streaming, integração de dados e aplicativos de missão crítica.

Entregue mensagens com taxa de transferência limitada pela rede usando um cluster de máquinas com latências tão baixas quanto 2 ms.

Escale **clusters** de produção até mil agentes, trilhões de mensagens por dia, petabytes de dados......... Expanda e contraia de forma elástica o armazenamento e o processamento.

Armazene fluxos de dados com segurança em um cluster distribuído, durável e tolerante e falhas.

Estique clusters de forma eficiente em zonas de disponibilidade ou conecte clusters separados em regiões geográficas.

Processamento de fluxo integrado (Processe fluxos de eventos com junções, agregações, filtros, transmissões usando processamento de tempo de evento e exatamente uma vez)

Conecte-se a quase tudo (A interface Connect pronta para uso do Kafka integra-se a centenas de fontes de eventos e coletores de eventos, incluindo Postgres, JMS, Elasticsearch, AWS S3 e mais)

Leia, escreva e processe fluxos de eventos em uma vasta gama de linguagens de programação.

grande ecossistema de ferramentas de código aberto: aproveite uma vasta gama de ferramentas pela comunidade.


## O que é Streaming de eventos?

Tecnicamente falando, 
É a prática de capturar dados em tempo real de fontes de eventos como banco de dados, sensores, dispositivos móveis, serviços em nuvem, aplicativos de software na forma de fluxos de eventos; 

Armazenar esses fluxos de eventos de forma durável para recuperação posterior; 

Manipular, processar e reagir aos fluxos de eventos em tempo real, bem como retrospectivamente; e roteamento dos fluxos de eventos para diferentes tecnologias de destino, conforme necessário. O Streaming de eventos garante, assim, um fluxo contínuo, conforme necessário. 

O streaming de eventos garante, assim, um fluxo contínua e interpretação de dados pra que a informação certa esteja no lugar certo, na hora certa.

Pode ser usado, por exemplo para processar pagamentos e transações financeiras em tempo real, como em bolsa de valores, bancos e seguradoras.

## COMO O KAFKA FUNCIONA? 

Kafka é um sistema distribuído que consiste em **servidores** e **clientes** que se comunicam por meio de um **protocolo de rede TCP**.
___

Um **evento** registra o fato de que "algo aconteceu" na sua empresa.
Conceitualmente, um evento tem uma chave, valor, timestamp e cabeçalhos de metadados opcionais.

```
Chave do evento: "Alice"
Valor do evento: "Fiz um pagamento de R$ 200 para Bob"
Carimbo de data/hora do evento: "25 de junho de 2020 às 14h06"
```

Os **producers** são os aplicativos clientes que publicam(gravam) eventos no kafka
Os **consumers** são aqueles que assinam (leem e processam) esses eventos.

Eles são totalmente desacoplados e agnósticos um do outro.

---

### Protocolo de rede TCP/IP
O protocolo TCP/IP é um *Grupo de protocolos de comunicação cujo objetivo é entregar pacotes de dados entre dispositivos de origem e destino, usando informações de endereço*.
[PROTOCOLO TCP/IP](https://www.hostgator.com.br/blog/o-que-e-protocolo-tcp-ip/)

O **IP**(Internet Protocol) é o “CPF” dos computadores.  
É o principal protocolo de comunicação responsável tanto pelos formatos quanto pelas regras de troca de dados e mensagens entre computadores de uma ou várias redes conectadas à internet. Cada dispositivo possui um endereço IP que o identifica, permitindo que ele se comunique e troque dados com outros dispositivos conectados.

 O **TCP**(Transmission Control Protocol) é responsável pela entrega de dados assim que o endereço IP for encontrado. Antes de transmitir os dados, o TCP estabelece uma conexão entre uma origem e um destino, que permanece ativa até o início da comunicação. 

Em seguida, ele divide grandes quantidades de dados em pacotes menores. Basicamente, o TCP é um padrão de comunicação que permite que programas, aplicativos e dispositivos de computação troquem mensagens em uma rede. 

**RELER TUDO NO LINK A CIMA**