# Java JRE e JDK: compile e execute o seu programa

Arquivo.java ->\COMPILA JDK/ -> Arquivo.class (bytecode) -> \JVM/ -> Mac/Linux/etc

Com o Java não é preciso reescrever ou adaptar o código para rodar em um outro SO. Temos um único executável (bytecode) para todos os sistemas, desde que exista a JVM.

Java Possui Muitas bibliotecas que só aumentam devido contribuições da comunidade open source.

O executável do mundo java (bytecode) precisa da JVM, mas é portável ( pode ser executado em vários SO )

O executável do Windows (.exe) funcionam apenas no windows

**PORQUE BYTECODE**?
Existe um conjunto de comandos que a **JVM** entente, chamados de **opcodes** (Operation Code), e cada opcode possui o tamanho de exatamente 1 Byte. E aí temos um **opcode de 1 Byte**, ou, mais simples, Bytecode. 
___

Para executar uma aplicação Java, apenas, basta o JRE
O JDK são as ferramentas de desenvolvimento mas também tem JRE embutido.

JRE = JVM + Bibliotecas

- **javac** Programa.java (COMPILA)
- **java** Programa (EXECUTA)
	
- Durante a compilação acontece uma verificação sintática do código fonte
- O compilador gera o Bytecode casp não tenha nenhum erro sintático no código fonte.
___
O Java é estaticamente e fortemente tipada, ou seja, precisa ser declarado o tipo da variável.

```
int idade = 24;

double salario = 1270.50;
int valor = (int) salario;
```
(int) -> **Casting**. Você está reafirmando para o compilador que você quer que o resultado seja um **int**, o que pode acarretar em perdas.