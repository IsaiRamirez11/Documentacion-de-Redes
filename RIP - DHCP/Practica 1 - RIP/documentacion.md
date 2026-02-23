
## Si desean copiar la practica asi como los scripts recuerden cambiar el dominio del DNS y engeneral revisar la parctica ya que esta practica tiene mi nombre por lo que les pido remplacen por el de ustendes, tanto dentro del servidor - services - DNS - ahi esta mi nombre y tanto en la configuracion del router en el domain-name ya que se encuentra con el dominio  isai.com que hace referencia a mi nombre 
##  Implementación de RIP v2

En cada router configuré:

 router rip

 version 2

 no auto-summary

Usé **RIP versión 2** porque la topología maneja múltiples subredes /24 y enlaces /30, así que necesitaba soporte para VLSM.  
Desactivé el auto-summary porque las redes están segmentadas en distintos bloques (172.16.x.x y 192.168.x.x), y no quería que se resumieran automáticamente a clases mayores.



##  Participación de interfaces en RIP

En 


 network 10.0.0.0

  se uso para incluir todos los enlaces seriales (10.1.1.0, 10.2.2.0, 10.3.3.0 y 10.4.4.0). ya que es mas facil que ir  una por una, mas que eso es por que investigando un poco mas me di cuenta que RIP solo ve la red mas fuerte por lo que era mejor usar este metodo





#

![Referencia a imagen de los comandos](img/topologia.png)
![Referencia a imagen de los comandos](img/pings.png)