# Cloud Architecture Design principles

## Design à prova de falhas
Entenda como e quais componentes falham e como arquitetar falhas para adicionar resiliência.

Exemplo simples: Construir um aplicativo que poderia ser executado em um único servidor, mas usando pelo menos dois servidores. Nesse cenário, voce estaria projetando sua arquitetura com a falha de seu servidor único como algo a se considerar

## Componentes desacoplados VS Arquitetura monolítica

Arquitetura Monolítica => Quando todos os processos são fortemente acoplados ou conectados e executados como um único serviço.  
Um problema que pode surgir com esse design é que se um aplicativo apresentar um pico de demanda, a arquitetura inteira deverá ser dimensionada. 

Do outro lado, temos componentes desacoplados. Em caso de um pico de demanda, por exemplo, é mais fácil dimensionar e corrigir as falhas

## Implemente elasticidade na nuvem VS On-premises
Elasticidade é um motivo comum para construir na nuvem. 

Em um ambiente On-premises, se a demanda aumentar depois que vocÊ implementou atualmente, o gerenciamento dessa demanda adicional será muito difícil.

## Pense paralelo
O Pensamento paralelo é semelhante ao desacoplamento, 

---

## Qual das opções representa um princípio de projeto da AWS Cloud?

A) Implementar pontos únicos de falha
B) **Implementar acoplamento fraco**
C) Implementar projeto monolítico
D) Implementar scaling vertical
