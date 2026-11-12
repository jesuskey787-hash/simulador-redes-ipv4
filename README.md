# Simulador de Redes IPv4 — Subnetting y LAN

Simulador educativo e interactivo desarrollado en **Unity** y publicado en **WebGL** para aprender conceptos básicos de redes informáticas mediante cálculos de direccionamiento IPv4 y una representación visual de una red local.

La aplicación está dividida en **dos partes independientes**: una calculadora de subredes a la izquierda y un simulador visual de una red LAN a la derecha. Permiten relacionar la teoría con una representación práctica de los dispositivos conectados.

## Probar el simulador online

🎮 **[Abrir simulador de redes IPv4 (Unity WebGL)](https://jesuskey787-hash.github.io/simulador-redes-ipv4/)**

Puedes probarlo directamente desde el navegador, sin instalar ningún programa.

## 1. Calculadora de subredes IPv4 (lado izquierdo)

Permite modificar el **prefijo CIDR** mediante un control deslizante y ver cómo cambian automáticamente los datos de una subred:

- **Dirección de red:** identifica la subred calculada.
- **Máscara de subred:** muestra la máscara en formato decimal, por ejemplo `255.255.255.0`.
- **Broadcast:** indica la dirección de difusión de la subred.
- **IP utilizables:** muestra cuántas direcciones pueden asignarse a equipos.
- **Prefijo CIDR:** permite experimentar con valores como `/22`, `/24` o `/28`.

**Objetivo:** comprender el *subnetting* y cómo influye la máscara en el tamaño de la red y el número de direcciones disponibles.

## 2. Simulador visual de red local (LAN) (lado derecho)

Representa una red local con un router, ordenadores, portátiles e impresoras.

- **Arrastrar y soltar:** mueve los dispositivos con el ratón desde las zonas **CABLE** y **WIFI** hasta el área de red.
- **Añadir o quitar equipos:** utiliza los botones `+` y `−` disponibles para modificar la cantidad de dispositivos.
- **Direcciones IP:** visualiza las IP asignadas o los intervalos utilizados por los equipos.
- **Router:** representa la puerta de enlace de la LAN (`192.168.1.1/24`).
- **Internet:** se representa mediante una IP pública de ejemplo (`212.15.70.2`).
- **Tipos de conexión:** identifica los dispositivos conectados por cable y por WiFi.

### Leyenda de conexiones

- **Línea continua:** conexión por cable (**Ethernet**).
- **Línea discontinua:** conexión inalámbrica (**WiFi**).

**Objetivo:** comprender cómo se organiza una red local, qué dispositivos forman parte de ella y cómo se representan sus conexiones.

## Cómo utilizar el simulador

1. Mueve el control deslizante de la izquierda y observa los cálculos de la subred.
2. En la parte derecha, arrastra dispositivos con el ratón desde **CABLE** o **WIFI** hasta el área de red.
3. Utiliza los botones `+` y `−` para cambiar la cantidad de equipos, cuando estén disponibles.
4. Observa sus direcciones IP y las líneas que indican el tipo de conexión.

> **Importante:** ambas partes son independientes. Cambiar el prefijo CIDR de la calculadora **no modifica** la configuración de la LAN representada a la derecha, que se muestra como `192.168.1.0/24`.

## Tecnologías utilizadas

- **Unity** y **C#**.
- **Unity UI** y **TextMeshPro**.
- **WebGL**, para ejecutar el simulador directamente en el navegador.

## Finalidad educativa

El proyecto busca facilitar el aprendizaje introductorio del direccionamiento IPv4, las máscaras de subred, el broadcast, las direcciones IP utilizables y la estructura de una red LAN. Se trata de una **simulación visual**, no de una herramienta que configure redes o establezca conexiones reales.
