# Hierarquia de Diretórios no Linux [Guia Básico]

No sistema de arquivos de uma forma geral, os objetos são organizados de uma formaa hierárquica e cada objeto possui uma identificação única dentro de uma tabela.

No linux, essa identificação é conhecida como **inode**.  
Ele carrega as informações de onde o objeto está localizado no disco, informações de segurança, data e hora de criação e última modificação dentre outras.

No Linux, tudo é um arquivo e, dependendo do seu tipo, pode se tornar um arquivo comum, um diretório, um link, um socket, um condutor, etc...

O Sistema de arquivos é semelhante a uma árvore de cabeça pra baixo. No topo, um direório Raiz (root) identificado como o sinal '/'. (NÃO CONFUNDIR COM O SUPERUSUARIO ROOT).

Essa estrutura é definida por um padrão de mercado chamado **Filesystem Hierarchy Standard** ou **FHS**, criado pela comunidade Linux em 1994 e mantida pela Linux Foundation.


```

                                     [ROOT] (/)
                                        |
   /     /      /     /     /     /     |     \      \     \       \     \     \     \
[bin] [boot] [dev] [etc] [home] [lib] [mnt] [opt] [proc] [root] [sbin] [tmp] [usr] [var]
                   |
                  / \
             [user1] [user2]
            

```