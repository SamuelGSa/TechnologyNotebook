## Contêineres
Uma maneira comum de empacotar códigos, configurações e dependências do aplicativo em um único objetivo

[-------Aplicativo A -----] [------ Aplicativo B -----]  
[Compartimentos/Biblioteca] [Compartimentos/Biblioteca]  
[--------------- Sistema Operacional -----------------]  
[-------------------- Servidor -----------------------]

Um host com vários contêineres, dezenas de hosts com dezenas de contêineres.  
os serviços de orquestração ajudam a implantar, gerenciar e dimensionar os aplicativos de contêineres

[-][-] [-][-] [-][-] [-][-]
[-][-] [-][-] [-][-] [-][-]
[----] [----] [----] [----]
[----] [----] [----] [----]

# ECS - Amazon Elastic Container Service
Sistema de gerenciamento de contêineres altamente dimensionável e de alto desempenho que permite executar e dimensionar aplicativos em contêineres na AWS .

# EKS - Amazon Elastic Kubernetes Service
Kubernetes é um software de código aberto que permite implantar e gerenciar aplicativos em contêineres em grande escala.

# AWS Fargate
Mecanismo de computação sem servidor para contêineres. Funciona com ECS e EKS.

Com Fargate, voce nao precisa provisionar ou gerenciar servidores. 