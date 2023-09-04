# Resources for Security Support

Encontre mais informações no AWS Knowledge Center, no Security Center e nos blogs e fórum de segurança da AWS. 

## Qual serviço ou recurso da AWS pode ser usado para impedir ataques de injeção SQL?

A) Grupos de segurança 
B) ACLs de rede
C) **AWS WAF**
D) Política do IAM

AWS WAF ou web Application Firewall é um firewall que pode filtrar tráfego com base em qualquer parte da localização, como endereços IP, cabeçalhos HTTP, Corpo HTTP ou cadeias de caracteres URI. Isso significa que ele pode filtrar qualquer solicitação que tenha um código SQL.

Grupos de segurança são firewalls de nível de instância que podem permitir que uma solicitação acesse uma instância do EC2.
Os grupos de segurança permitem o tráfego com base em: Porta, Protocolo, Origem ou destino, no entanto, eles não podem inspecionar um pacote HTTP.  
Grupos de segurança estão em nível de **instância**

ACLs de rede controlam o tráfego com base em: Tipo de tráfego, Porta, Protocolo, Origem ou destino.  
ACLs de rede estão em nível de **sub-rede**

As politicas do IAM são anexadas às entidades da AWS, como usuários, grupos ou perfis do IAM. Essas políticas determinam quais ações da AWS podem ou não ser executadas. 