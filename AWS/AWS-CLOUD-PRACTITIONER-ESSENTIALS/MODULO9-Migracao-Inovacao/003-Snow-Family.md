# AWS Snow Family
Uma coleção de dispositivos físicos para transporte físico de até exabytes de dados para dentro e para fora da AWS. 

Consiste nos serviços:

![Snow Family](../../../_images/AWS-Cloud-Practitioner-Essentials/Modulo9/snowFamily.jpg)

## AWS Snowcone
é um dispositivo pequeno, robusto e seguro para transferência de dados e computação de borda.

Ele tem 2 CPUs, 4 GB de memória e 8 TB de armazenamento utilizável.

## AWS Snowball 
oferece dois tipos de dispositivos: os dispositivos

- **Snowball Edge otimizados para armazenamento**: ideais para migrações de dados de grande escala e fluxos de trabalho de transferência recorrentes, em além da computação local com necessidades maiores de capacidade.  
  **Armazenamento**: 80 TB de capacidade de disco rígido (HDD) para volumes de blocos e armazenamento de objeto compatível com o Amazon S3, além de unidade de estado sólido (SSD) de 1 TB para volumes de blocos.  
  **Computação**: 40 vCPUs e 80 GiB de memória para dar suporte a instâncias sbe1 do Amazon EC2 (equivalente a C5).

- **Snowball Edge otimizado para computação**: fornece recursos de computação poderosos para casos de uso, como machine learning, análise de vídeo em movimento completo, análise e pilhas de computação locais.  
  **Armazenamento**: capacidade de HDD utilizável de 42 TB para armazenamento de objeto compatível com o Amazon S3 ou volumes de blocos compatíveis com o Amazon EBS e também 7,68 TB de capacidade de SSD NVMe utilizável para volumes de blocos compatíveis com o Amazon EBS.   
  **Computação**: 52 vCPUs, 208 GiB de memória e uma GPU NVIDIA Tesla V100 opcional. Os dispositivos executam as instâncias sbe-c e sbe-g do Amazon EC2, que são equivalentes às instâncias C5, M5a, G3 e P3.

## AWS Snowmobile
Serviço de transferência dados na escala de exabytes usado para mover grandes quantidades de dados para a nuvem AWS.

Você pode transferir até 100 petabytes por Snowmobile, um contêiner de transporte reforçado com 13,71 metros de comprimento puxado por um caminhão semirreboque.