# CRUD do Ozelo

Fazer u CRUD de um registro Simples (Cadastro de Cliente) usando REST e H2
___

h2 -> É um banco de Dados embutido , de código aberto  e na memória.
Sistema de gerenciamento de banco de dados relacional.

Configurando o h2 (em application.properties)

___

O mapeamento objeto-relacional foi criado para abstrair as diferenças entre o modelo relacional e o paradigma orientado a objetos. Assim, deixa de ser necessário criarmos soluções com o intuito de converter dados em objetos e vice-versa.

Em Java, após a especificação JPA, isso passou a ser feito pelos frameworks que a implementam, como o Hibernate, EclipseLink e OpenJPA. A nós, desenvolvedores, basta fazer uso das anotações disponibilizadas pela JPA para viabilizar o mapeamento, evitando dessa forma criar uma forte dependência com alguma implementação.
--- 
@Entity - é utilizada para informar que uma classe também é uma entidade.
Uma entidade representa, na Orientação a Objetos, uma tabela do banco de dados, e cada instância dessa entidade representa uma linha dessa tabela.

A anotação @Id é uma anotação obrigatória e determina qual campo da entidade representa a chave primária da tabela no banco de dados.

___
JPA é um framework leve, baseado em POJOS (Plain Old Java Objects) para persistir objetos Java. A Java Persistence API, diferente do que muitos imaginam, não é apenas um framework para Mapeamento Objeto-Relacional (ORM - Object-Relational Mapping), ela também oferece diversas funcionalidades essenciais em qualquer aplicação corporativa.

(POJOS - são objetos Java que seguem um desenho extremamente simplificado)
___
@Repository - as classes do Spring Repository são detectadas automaticamente pela estrutura do spring por meio da verificação do caminho de classe.
 se você estiver usando Spring Data para gerenciar operações de banco de dados, deverá usar a interface Spring Data Repository..

@Autowired - Ele permite que o psring resolva e injete beans de colaboração em nosso bean 




bean????????

@AllArgsComstructors
@NoArgsConstructors
@Data
@Builder

Person.builder().email().nome().build();

Persons/ identificador

trocar  identificador de inteiro para String 

filtro por queryString 

Colocar campo data com data e hora 
e filtrar por ele tambem. 
ex: entre datas e maior e menor datas