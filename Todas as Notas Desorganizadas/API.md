# API - Application Programming Interface ( Interface de Programação de Aplicações)
Conjunto de rotinas e padrões estabelecidos e documentados por uma aplicação A, para que outras aplicações consigam utilizar as funcionalidades desta aplicação A, sem precisar conhecer detalhes da implementação do software.

APIs permitem uma interoperabilidade entre aplicações.  
Em outras palavras, a comunicação entre aplicações e entre os usuários.

Aceita a linguagem XML, JSON e YAML

## Representação XML
```
<endereco>
    <rua>
    Rua Recife
    </rua>
    <cidade>
    Paulo Afonso
    </cidade>
</endereco>
```

## Representação JSON
```
{ endereco:
    {
    rua: Rua Recife
    cidade: Paulo Afonso
    }
}
```

## Representação YAML
```
endereco:
rua: Rua Recife
cidade: Paulo Afonso
```

---

# REST - Representational State Transfer (Transferência de Estado Representacional)
Consiste em princípios/regras/constraints que, quando seguidas, permitem a criação de um projeto com interfaces bem definidas. Desta forma, permitindo, por exemplo, que aplicações se comuniquem.

## REST x RESTful
 A diferença é apenas gramatical. Em outras palavras, sistemas que utilizam os princípios REST são chamados de RESTful.

- REST: conjunto de princípios de arquitetura
- RESTful: capacidade de determinado sistema aplicar os princípios de REST.