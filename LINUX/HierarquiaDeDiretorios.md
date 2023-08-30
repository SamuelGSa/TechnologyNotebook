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

### / 
Diretorio raiz do Sistema de Arquivos

### /bin
Contem os comandos que podem ser utlizados pelos usuários e pelo adm do sistema. São requeridos no modo monousuario ou de manutenção (single-user-mode) e tambem podem conter comandos que são utilizados indiretamente por alguns scripts.  
Contém arquivos executáveis, como: 
   - cat, chgrp, chmod, chown, cp, date, dd, df, dmesg, echo, hostname, kill, ln, more, mount, mv, ps, pwd, rm, rmdir, sed, su, umount e uname;

### /boot 
Arquivos estáticos necessários para iniciar o Sistema. É onde fica localizada a imagem do Kernel, initramfs e alguns arquivos do Grub.

### /dev 
Abstração do Kernel onde ficam os arquivos para acesso do dispositivos do sistema, omo discos, cd-roms, pendrives, etc. Esse diretório é um pseudo-filesystem, e nao existe no disco.

### /etc
Arquivos necessários para configuração do sistema. Necessários para a carga do SO.Ele possui arquivos importantes tais como: 
 - fstab, exports, passwd, shadow, group, hosts, hosts.allow, hosts.deny, inittab, ld.so.conf, mtab, profile, services, etc.

   Nele também residem os arquivos de configuração das interfaces de rede.

### /home
Nesses Diretórios localizam-se scripts de carga de perfil e do shell de cada usuario.

### /lib 
Arquivos de bibliotecas essenciais ao sistema. Utilizadas pelos programas em /bin e módulos do Kernel.

### /mnt
Diretório vazio utilizado como ponto de montagem de dispositivos na máquina. Usado pelo administrador para montar discos.

### /media
Diretório vazio utilizado como ponto de montagem de dispositivos na máquina, tais como cdrom, dvd, pendrives, etc.

### /proc 
Informações do Kernel e dos processos. É um pseudo-filesystem e não existe realmente no disco. Neste diretório ficam as abstrações de descritores de tudo quanto há no Kernel do sistema. É possível não só ler os dados, bem como fazer alterações no comportamento do Kernel alterando o conteúdo de arquivos em /proc.  
'Fazendo uma abstração do Windows, este diretório seria o “registro” do sistema'.

### /opt 
Neste diretório ficam instalados os aplicativos que não são da distribuição do Linux.
- banco de dados de terceiros, software de vetores Cad, etc.

### /root
Diretório home do superusuário root. Dependendo da distribuição pode estar presente ou não;

### /run 
Este diretório contém informações do sistema desde a última carga. Os arquivos deste diretório são apagados ou zerados no início do processo de boot. Arquivos como aqueles que indicam o PID do processo em execução devem residir neste diretório.

### /sbin 
Arquivos essenciais ao sistema, como aplicativos e utilitários para a administração da máquina. Normalmente só o superusuário tem acesso a estes arquivos, 
- fdiskm fsck, ifconfig, init, mkfs, mkswap, route, reboot, swapon e swapoff.

### /tmp 
Diretório de arquivos temporários. Em algumas distribuições este diretório é montado em memória. Recomenda-se que seu conteúdo seja apagado de tempos em tempos ou a cada reboot. 

### /usr 
Arquivos pertencentes aos usuários e a segunda maior hierarquia de diretórios no Linux.

### /var
Diretório onde são guardadas informações variáveis sobre o sistema, como arquivos de log, arquivos de e-mail etc. Possui subdiretórios importantes
 - **/var/cache** : mantém informações de cache das aplicações como cálculos, etc;
 - **/var/lib** : mantém informações de estado das aplicações;
 - **/var/lock** : mantém arquivos de trancamento que retém dispositivos para uso exclusivo de alguma determinada aplicação;
 - **/var/log** : mantém os arquivos de log do sistema, tais como messages, lastlog e wtmp.
 - **/var/mail** :   mantém os diretórios de contas de email dos usuários;
 - **/var/opt** : mantém os arquivos variáveis das aplicações;
 - **/var/spool** : mantém dados de processos que mantém filas de arquivos, tais impressão e saída de email;
 - **/var/tmp** : mantém os arquivos temporários das aplicações que precisem ser preservados entre o reboot do sistema