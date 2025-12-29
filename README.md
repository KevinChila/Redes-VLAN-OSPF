# Proyecto de Redes VLAN y OSPF - Cisco Packet Tracer

## Descripción
Este proyecto fue realizado en Cisco Packet Tracer y simula una red empresarial con múltiples VLANs y enrutamiento OSPF. El objetivo principal es demostrar la segmentación de la red mediante VLANs, el enrutamiento inter-VLAN usando Router-on-a-Stick, y la conectividad entre redes locales y remotas.

## Topología
- **Switches**: Configurados con varias VLANs (10, 20, 30) y puerto trunk.  
- **Routers**: Configuración OSPF para el enrutamiento entre VLANs y conexión a red remota.  
- **PCs**: Asignadas a diferentes VLANs para pruebas de conectividad.  

## VLANs
| VLAN | Nombre       | PC asignada |
|------|-------------|------------|
| 10   | RED_VLAN10  | PC1        |
| 20   | RED_VLAN20  | PC2        |
| 30   | RED_VLAN30  | PC3        |

## Pruebas realizadas
1. **Ping entre VLANs**  
   - Desde PC1 (VLAN 10) a PC2 (VLAN 20) y PC3 (VLAN 30) ✅  
2. **Ping a red remota**  
   - Desde PC1 a PC4 (172.16.1.10) ✅  
3. **Ping a Internet (Loopback)**  
   - Desde cualquier PC a 8.8.8.8 ✅  

## Comandos importantes utilizados
- `show vlan brief` → Verifica las VLAN configuradas en el switch.  
- `show running-config` → Muestra la configuración actual del dispositivo.  
- `show interfaces trunk` → Verifica los puertos trunk y las VLANs permitidas.  
- `ping <IP>` → Prueba la conectividad entre dispositivos.  
- `show ip route` → Visualiza las rutas OSPF y conectadas en el router.  
- `show ip ospf neighbor` → Verifica los vecinos OSPF y el estado de la relación.  

## Archivo del proyecto
- El archivo de Packet Tracer está incluido en este repositorio: `Actividad1_Chila_Kevin.pkt`  
- **Para descargarlo:** ingresa al archivo en GitHub y da clic en **"View raw"**, luego guarda el archivo en tu computadora.  

---

Hecho por: KEVIN CHILA  
Universidad Politécnica Salesiana
