# Simulación de Enrutamiento BGP - Cisco Packet Tracer

Este proyecto muestra una red simulada de 3 organizaciones interconectadas usando el protocolo BGP (Border Gateway Protocol), con asignación de AS (Sistema Autónomo) y uso de interfaces loopback para identificación del router.

## Topología de Red

- **Contabilidad (AS 65010)** - Red interna: 192.168.1.0/24
- **Soporte TI (AS 65020)** - Red interna: 192.168.2.0/24
- **Administración (AS 65030)** - Red interna: 192.168.3.0/24

Los routers están interconectados con redes punto a punto y utilizan loopbacks como `router-id` para establecer relaciones BGP.

## Tecnologías utilizadas

- Cisco Packet Tracer
- BGP (Basic Configuration)
- Subnetting
- Interfaces Loopback
- Comunicación inter-AS

## Archivos incluidos

- `BGP.pkt`: Archivo del proyecto en Packet Tracer
- Configuraciones de los tres routers
- Captura de la topología

##  Cómo probarlo

1. Abre `BGP.pkt` con Cisco Packet Tracer.
2. Haz ping entre PCs de distintas áreas (ej. PC0 → PC3) para verificar conectividad.
3. Verifica las rutas BGP con:
       show ip bgp 
       show ip route
