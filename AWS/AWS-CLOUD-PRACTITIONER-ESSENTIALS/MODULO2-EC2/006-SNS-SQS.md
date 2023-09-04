Se 'B' estiver Offline, 'A' começa a ter problemas em entregar as mensagens. Dessa forma, a arquitetura está **altamente acoplada**.

[APLICAÇÃO A] -------> [APLICAÇÃO B]

---

Com uma  **arquitetura de acoplamento flexível**, uma única falha não causará falhas em cascata 

[APLICAÇÃO A] -------> [FILA DE MENSAGENS] -------> [APLICAÇÃO B]

# SNS - Amazon Simple Notification Service
Serviço de publicação/Assinatura. Usando tópicos do SNS, um editor publica mensagens para assinantes.

No SNS, os **assinantes** podem ser servidores web, endereços de E-mail, funções do AWS LAMBDA e outras opções.

>O Operador do caixa entrega os pedidos ao barista, que prepara a bebida.

# SQS - Amazon Simple Queue Service
Serviço de enfileiramento de mensagens. Use para enviar, armazenar e receber mensagens entre componentes de software sem perder mensagens ou precisar que outros serviços estejam disponíveis.

---

## Computação sem servidor (Serverless)
Significa que o código é executado em servidores, sem quem você precise provisionar ou gerenciar esses servidores.
AWS Lambda, é um exemplo de computado Serverless.
