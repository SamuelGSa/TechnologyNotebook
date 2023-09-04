# Interfaces Java

Uma interface é similar a um contrato, através dela podemos especificar quais métodos as classes que implementam esta interface são obrigados a implementar.

**exemplo**: 

```
public interface Terrestre {

     final int QUADRUPEDE = 4;
     abstract String andar(String direcao);
}
```
Todo método de uma interface é abstrato. Quer dizer que ele não é implementado.

- final == Constante.

```
public class Cachorro implements Terrestre {

     @Override
     public String andar(String direcao) {
          return "Indo para " + direcao + "... Wolf Wolf ...";

     }

}
```
- pode ser implementado +1 interface

```
public class PrincipalInterface {

     public static void main (String[] args) {
          Cachorro cao = new Cachorro();
          String resp = cao.andar("norte");
          System.out.println(resp)
     }
}

Run: Indo para norte... Wolf Wolf ...
```

- Cachorro cao = ...
- Terrestre cao = ... 
- Funciona igual. Todo cao é terrestre (Do tipo Interface)