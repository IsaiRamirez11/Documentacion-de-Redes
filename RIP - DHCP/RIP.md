# RIP – Routing Information Protocol

## ¿Qué es RIP?

**RIP (Routing Information Protocol)** es un protocolo de enrutamiento dinámico de tipo *Distance Vector* utilizado en redes IP para intercambiar información de rutas entre routers.


---


## ¿Cómo funciona RIP?

### 1. Envío de actualizaciones

Cada 30 segundos, los routers envían su tabla completa de enrutamiento a sus vecinos directamente conectados.

### 2. Cálculo de la mejor ruta

RIP utiliza el número de saltos como métrica:

 Cada router atravesado cuenta como 1 salto.
La ruta con menor número de saltos es la elegida.

### 3. Actualización de tabla

Si un router recibe una ruta con menor número de saltos que la actual, actualiza su tabla de enrutamiento.

---


## Versiones de RIP

### RIPv1
- Protocolo classful
- No soporta VLSM
- No envía máscara de subred

### RIPv2
- Protocolo classless
- Soporta VLSM y CIDR
- Envía máscara de subred
- Permite autenticación

