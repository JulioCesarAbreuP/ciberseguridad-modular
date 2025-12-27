Ataques en la capa 2 del modelo OSI y sus contramedidas modernas



La capa 2 del modelo OSI —Enlace de Datos— es uno de los territorios más críticos y, paradójicamente, más ignorados en ciberseguridad. Mientras muchos profesionales centran su atención en firewalls, cifrado o vulnerabilidades de aplicaciones, la Capa 2 permanece como un campo de batalla silencioso donde se libran ataques que pueden comprometer toda la arquitectura de red sin generar alertas visibles.

Aquí no se explotan CVEs ni se fuerzan contraseñas.  

Aquí se manipula la identidad misma de los dispositivos, se envenenan tablas, se suplanta información y se altera el flujo natural del tráfico. Es un ataque a la confianza fundamental de la red.



¿Por qué es tan crítica la Capa 2?

Porque es la capa donde los dispositivos se reconocen entre sí, es el nivel donde se decide:

- quién es quién,  
- quién puede hablar con quién,  
- y cómo se mueve el tráfico dentro de un segmento.

Si un atacante logra manipular esa identidad, puede:

- Redirigir tráfico sin ser detectado  
- Interceptar comunicaciones legítimas  
- Suplantar dispositivos críticos  
- Romper la integridad de la red  
- Preparar ataques más avanzados en capas superiores  
- Desplegar ataques de movimiento lateral sin generar ruido
- 

La Capa 2 es el puente levadizo del castillo:  si alguien lo falsifica, puede entrar sin que nadie lo note.


Ataques comunes en la Capa 2



1. MAC Spoofing

El atacante cambia su dirección MAC para hacerse pasar por otro dispositivo legítimo.

Esto permite:

- Evadir controles de acceso  
- Interceptar tráfico destinado a otro equipo  
- Acceder a VLANs restringidas  
- Saltar políticas basadas en identidad de dispositivo  


En entornos corporativos, este ataque puede comprometer:

- impresoras,  
- teléfonos VoIP,  
- cámaras IP,  
- o incluso switches de acceso.


2. ARP Poisoning (Envenenamiento ARP)

- El atacante envía respuestas ARP falsas para asociar su MAC con la IP de otro equipo.



Consecuencias:

- Intercepción de tráfico (Man-in-the-Middle)  
- Redirección maliciosa  
- Pérdida de integridad  
- Robo de credenciales  
- Manipulación de sesiones  


Este ataque es especialmente peligroso porque:

- No requiere privilegios elevados  
- No genera logs en la mayoría de sistemas  
- Funciona en redes planas o mal segmentadas  


3. CAM Table Overflow

- El atacante satura la tabla CAM del switch con direcciones MAC falsas haciendolo comportar como un hub.



Cuando la tabla se llena:

- El switch deja de comportarse como switch  
- Empieza a difundir tráfico como un hub  
- El atacante puede capturar paquetes de otros dispositivos  


Este ataque es ideal para:

- Capturar tráfico sensible  
- Preparar ataques posteriores  
- Romper la confidencialidad de la red  


4. VLAN Hopping

- El atacante manipula tramas 802.1Q para saltar entre VLANs.



Esto permite:

- Acceder a segmentos aislados  
- Alcanzar servidores o dispositivos críticos  
- Evadir segmentación lógica  


Es un ataque especialmente peligroso en redes donde:

- Se usan VLANs para separar entornos  
- No hay hardening en los puertos troncales  
- No se aplican políticas de aislamiento estrictas  


Contramedidas modernas



Las defensas en Capa 2 no son opcionales, son parte del mínimo viable de cualquier arquitectura seria.



- Port Security
    Limita cuántas MAC pueden conectarse a un puerto.  
    Evita suplantaciones y accesos no autorizados.



- Dynamic ARP Inspection (DAI)
    Valida las respuestas ARP.  
    Bloquea ARP poisoning automáticamente.



- DHCP Snooping
    Evita servidores DHCP falsos.  
    Protege la asignación de IPs y genera una base confiable para DAI.



- IP Source Guard
    Evita que un dispositivo use una IP que no le corresponde.



- NAC (Network Access Control)
    Autentica dispositivos antes de permitirles entrar a la red.  

    Controla quién entra, desde dónde y con qué nivel de confianza.



- Segmentación y VLANs
    Reduce el alcance de un ataque.  

    Evita que un atacante se mueva libremente.



- 802.1X + EAP
    Autenticación fuerte a nivel de puerto.  

    Ideal para entornos corporativos y redes sensibles.



- Hardening de puertos troncales
    Evita VLAN hopping y manipulación de tramas.



Lección doctrinal



La Capa 2 no es “baja” ni “simple”, es la base de todo. Si falla aquí, fallan todas las capas superiores.



 “Quien vigila la capa de enlace, protege la raíz del castillo.”


Conclusión

Los ataques en la Capa 2 son silenciosos, efectivos y peligrosos. Pero con las contramedidas adecuadas, la red se vuelve mucho más resistente y predecible.



Este artículo forma parte de mi proyecto https://pergamino-digital-ciberseguridad.blogspot.com/, donde documento conceptos, laboratorios y arquitecturas defensivas con un enfoque pedagógico y doctrinal.

Si tienes sugerencias, críticas o ideas para mejorar este contenido, estaré encantado de escucharlas.


