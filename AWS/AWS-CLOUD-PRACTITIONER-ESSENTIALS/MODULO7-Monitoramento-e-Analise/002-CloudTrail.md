# AWS CloudTrail

Registra as chamadas de API realizadas na sua conta. "Trilha de migalhas de pão" (ou um log de ações) que alguem deixou para trás.

Normalmente, os eventos são atualizados no CloudTrail dentro de **15 minutos** após uma chamada de API

## Exemplo: Evento do AWS CloudTrail

>Suponha que o proprietário da cafeteria esteja navegando pela seção AWS Identity and Access Management (IAM) do AWS Management Console
>
>Na seção Event History (Histórico de eventos) do CloudTrail, o proprietário aplica um filtro para exibir somente os eventos da ação da API “CreateUser” no IAM. O proprietário localiza o evento para a chamada de API que criou um usuário do IAM para Mary. Esse registro de evento fornece detalhes completos sobre o que ocorreu: 
>
>em 1º de janeiro de 2020, às 9:00, o usuário do IAM John criou um novo usuário do IAM (Mary) pelo AWS Management Console.

![Exemplo CloudTrail](../../_images/AWS-Cloud-Practitioner-Essentials/Modulo7/exemplo-cloud-trail.png)

## CloudTrail Insights

e recurso opcional permite que o CloudTrail detecte automaticamente atividades de API **incomuns** em sua conta AWS. 