

## ¿Cuál es el objetivo?

El objetivo es armar y hacer funcionar una red completa, como si fuera una red real de una empresa, donde todo se comunique correctamente aunque esté dividido en varias VLAN y en diferentes routers.

---

## 1. Separar la red con VLAN

Se crean varias VLAN para dividir la red en partes más pequeñas.  
Cada VLAN representa una red diferente.

Esto sirve para:
Organizar mejor la red
Evitar que todo esté en el mismo segmento
Controlar mejor el tráfico

---

## 2. Permitir comunicación entre VLAN

Como cada VLAN es una red distinta, necesitan un dispositivo que las enrute.

Aquí se practica:
 Router-on-a-Stick en los routers
 Interfaces VLAN (SVI) en el switch capa 3
 Configurar la puerta de enlace (.254 normalmente)

La idea es que equipos de diferentes VLAN puedan comunicarse.

---

## 3. Configurar DHCP

Se configuran pools DHCP para que las computadoras obtengan IP automáticamente.

En cada red se define:
 Rango de direcciones
 Gateway
 DNS
 Dominio

Con esto se evita configurar IP manualmente en cada equipo.

---

## 4. Usar enrutamiento dinámico (RIP v2)

Se activa RIP versión 2 para que:
 Los routers compartan sus redes automáticamente
 No sea necesario crear rutas estáticas
 Toda la topología pueda comunicarse

---

## 5. Integrar servicios reales

La red no solo enruta, también tiene:
 Servidor Web
 Servidor FTP
 Servidor DNS
 Servidor de correo

Esto permite comprobar que:
 Hay comunicación total
 El DNS resuelve nombres
 Se pueden enviar correos
 Se puede acceder a páginas web

---

## En resumen

Estas prácticas buscan que entiendas cómo funciona una red completa:

 Cómo se segmenta con VLAN
 Cómo se enruta entre redes
 Cómo se asignan IP automáticamente
 Cómo se intercambian rutas
 Cómo se conectan servicios reales dentro de la red