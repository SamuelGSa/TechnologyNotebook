# VAR - Type Inference

**Inferência de tipo** refere-se a um paradigma de linguagem de programação e usamo para definir nossos tipos de objetos e variáveis.

No JAVA, só veio na JDK 10.

### Sem o VAR
```
String nome = "Sergio Lopes";
LocalDateTime dateTime = LocalDateTime.now();
```

### Com o VAR
```
var nome = "Sergio Lopes";
var dateTime = LocalDateTime.now(); 
```

```
hashMap<Integer, String> mapa = new HashMap<Integer, String>();
```
```
var mapa = new HashMap<integer, String>();
```
Uma vantagem de se usar o VAR é que o código fica menos verboso, você delega para o complicador a decisão de determinar qual é o tipo da variável.

___
## Regras para usar este modelo: 

- São obrigadas a serem inicializadas.
- Limitado a variáveis locais.
- Em Arrays, você não pode abrir mão dos tipos de dado
- var letras new char[]{"A", "B", "C", "D", "E"};
- A troca de valores ou adição de valores de uma variável precisam ser do mesmo tipo
```
var tamanho = 9;
tamanho = 10.9;
```
