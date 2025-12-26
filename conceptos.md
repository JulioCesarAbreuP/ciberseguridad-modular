


Zero Trust

Definición técnica:  
Modelo de seguridad basado en verificación continua donde ningún usuario, dispositivo o red se considera confiable por defecto.

Propósito arquitectónico:  
Eliminar la confianza implícita y evaluar cada solicitud según identidad, contexto y riesgo.

Integración en sistemas:  
Se implementa mediante IAM, MFA, segmentación, políticas dinámicas y monitoreo continuo.

Aforismo:  
La confianza no se presupone; se renueva en cada acceso.

DNS

Definición técnica:  
Sistema distribuido que traduce nombres de dominio en direcciones IP para permitir el enrutamiento de tráfico.

Propósito arquitectónico:  
Separar identidad lógica de ubicación real y permitir escalabilidad y flexibilidad.

Integración en sistemas:  
Usado en resolución interna, balanceo por DNS, DNSSEC y servicios cloud.

Aforismo:  
Los nombres viajan donde las direcciones no alcanzan.

PKI

Definición técnica:  
Infraestructura que gestiona certificados digitales y claves públicas para autenticación, cifrado y firma.

Propósito arquitectónico:  
Establecer confianza verificable entre entidades distribuidas.

Integración en sistemas:  
Fundamento de TLS, firma digital, autenticación mutua, VPN y Zero Trust.

Aforismo:  
La confianza digital nace de una firma que todos reconocen.

OAuth 2.0

Definición técnica:  
Marco de autorización que permite delegar acceso a recursos sin compartir credenciales del usuario.

Propósito arquitectónico:  
Separar autenticación de autorización y controlar permisos entre servicios.

Integración en sistemas:  
Base de APIs modernas, aplicaciones móviles, SSO y flujos basados en tokens.

Aforismo:  
No compartas la llave; comparte el permiso.

EDR

Definición técnica:  
Tecnología que monitoriza endpoints para detectar comportamientos anómalos, responder a amenazas y registrar actividad.

Propósito arquitectónico:  
Proteger el punto más vulnerable de la infraestructura: el dispositivo del usuario.

Integración en sistemas:  
Se complementa con SIEM, XDR, Zero Trust y controles de identidad.

Aforismo:  
El perímetro ya no es la red; es cada dispositivo.

Microsegmentación

Definición técnica:  
Estrategia de seguridad que divide la red en segmentos extremadamente pequeños, aplicando políticas granulares basadas en identidad, aplicación o flujo.

Propósito arquitectónico:  
Limitar el movimiento lateral y contener incidentes dentro de dominios mínimos.

Integración en sistemas:  
Se implementa con firewalls distribuidos, SDN, Zero Trust y políticas basadas en contexto.

Aforismo:  
Cuando cada camino es estrecho, el atacante no avanza.

Subnetting

Definición técnica:  
Proceso de dividir una red IP en subredes más pequeñas mediante máscaras específicas.

Propósito arquitectónico:  
Optimizar el uso de direcciones, mejorar el rendimiento y aplicar políticas de seguridad por segmentos.

Integración en sistemas:  
Fundamental en diseño de redes, VLAN, routing y segmentación lógica.

Aforismo:  
Dividir bien es controlar mejor.

DHCP

Definición técnica:  
Protocolo que asigna direcciones IP y parámetros de red de forma automática a los dispositivos.

Propósito arquitectónico:  
Simplificar la administración de direcciones y evitar conflictos de configuración manual.

Integración en sistemas:  
Presente en redes corporativas, domésticas, cloud y entornos híbridos.

Aforismo:  
La red fluye cuando cada nodo recibe su identidad sin fricción.

ARP

Definición técnica:  
Protocolo que resuelve direcciones IP en direcciones MAC dentro de una red local.

Propósito arquitectónico:  
Permitir la comunicación entre dispositivos en la misma red física.

Integración en sistemas:  
Base del funcionamiento de switches, routers y comunicación LAN.

Aforismo:  
Para hablar con alguien, primero debes saber cómo encontrarlo.

Reverse Proxy

Definición técnica:  
Servidor que recibe solicitudes externas y las redirige a servidores internos, ocultando su estructura.

Propósito arquitectónico:  
Aislar servicios internos, distribuir carga y aplicar controles de seguridad.

Integración en sistemas:  
Usado en balanceadores, WAF, microservicios y arquitecturas web modernas.

Aforismo:  
La entrada visible no siempre revela el camino real.

SSO

Definición técnica:  
Mecanismo que permite a un usuario autenticarse una sola vez y acceder a múltiples servicios sin repetir credenciales.

Propósito arquitectónico:  
Reducir fricción, mejorar experiencia y centralizar control de identidad.

Integración en sistemas:  
IAM, aplicaciones empresariales, servicios cloud y entornos híbridos.

Aforismo:  
Una sola autenticación, múltiples puertas abiertas.

OpenID Connect

Definición técnica:  
Protocolo de autenticación basado en OAuth 2.0 que permite verificar la identidad del usuario mediante tokens.

Propósito arquitectónico:  
Unificar autenticación moderna en aplicaciones distribuidas.

Integración en sistemas:  
SSO, APIs, aplicaciones móviles y servicios cloud.

Aforismo:  
La identidad viaja ligera cuando se representa con un token.

FIDO2

Definición técnica:  
Estándar de autenticación sin contraseña basado en criptografía de clave pública y dispositivos seguros.

Propósito arquitectónico:  
Eliminar contraseñas y reducir ataques basados en credenciales.

Integración en sistemas:  
IAM, autenticación web, dispositivos biométricos y entornos Zero Trust.

Aforismo:  
La mejor contraseña es la que ya no existe.

Cifrado simétrico

Definición técnica:  
Método de cifrado donde la misma clave se usa para cifrar y descifrar datos.

Propósito arquitectónico:  
Proteger grandes volúmenes de información con alta eficiencia.

Integración en sistemas:  
TLS, almacenamiento cifrado, VPN y comunicaciones internas.

Aforismo:  
Una sola llave guarda y revela el mismo secreto.

Cifrado asimétrico

Definición técnica:  
Método de cifrado que utiliza un par de claves: una pública para cifrar y una privada para descifrar.

Propósito arquitectónico:  
Permitir intercambio seguro de claves, autenticación y firma digital.

Integración en sistemas:  
PKI, TLS, certificados, firma digital y autenticación mutua.

Aforismo:  
Una clave abre el mensaje; la otra demuestra quién eres.

Firma digital

Definición técnica:  
Mecanismo criptográfico que garantiza autenticidad, integridad y no repudio mediante claves públicas y privadas.

Propósito arquitectónico:  
Validar que un mensaje o documento proviene de quien dice ser y no ha sido alterado.

Integración en sistemas:  
PKI, correo seguro, documentos electrónicos, APIs y contratos digitales.

Aforismo:  
La identidad se demuestra con hechos, no con palabras.

Modelo OSI

Definición técnica:  
Modelo de referencia de siete capas que describe cómo se comunican los sistemas en una red.

Propósito arquitectónico:  
Estandarizar funciones de red para facilitar interoperabilidad, diagnóstico y diseño modular.

Integración en sistemas:  
Base conceptual para protocolos, firewalls, IDS, segmentación y análisis de tráfico.

Aforismo:  
Comprender la red es subir por capas sin perder el contexto.

Modelo TCP/IP

Definición técnica:  
Conjunto de protocolos que define cómo se transmiten datos en Internet, estructurado en cuatro capas funcionales.

Propósito arquitectónico:  
Implementar comunicación real entre sistemas distribuidos, desde la red hasta la aplicación.

Integración en sistemas:  
Fundamento de redes modernas, enrutamiento, NAT, VPN y servicios web.

Aforismo:  
No es un modelo teórico; es la carretera por donde viaja todo.

XDR

Definición técnica:  
Plataforma que unifica detección y respuesta en múltiples vectores: endpoints, red, nube y correo.

Propósito arquitectónico:  
Romper los silos de visibilidad y correlacionar amenazas en tiempo real.

Integración en sistemas:  
Complementa SIEM, EDR, NDR y herramientas de respuesta automatizada.

Aforismo:  
Ver todo, correlacionar todo, responder antes de que sea tarde.

NDR

Definición técnica:  
Tecnología que analiza tráfico de red para detectar amenazas mediante análisis de comportamiento y aprendizaje automático.

Propósito arquitectónico:  
Identificar ataques que no dejan huella en endpoints o logs tradicionales.

Integración en sistemas:  
Se conecta a switches, firewalls, SIEM y plataformas XDR.

Aforismo:  
La red no miente; solo hay que saber escucharla.

NDR

Definición técnica:  
Tecnología que analiza tráfico de red para detectar amenazas mediante análisis de comportamiento y aprendizaje automático.

Propósito arquitectónico:  
Identificar ataques que no dejan huella en endpoints o logs tradicionales.

Integración en sistemas:  
Se conecta a switches, firewalls, SIEM y plataformas XDR.

Aforismo:  
La red no miente; solo hay que saber escucharla.

Segmentación

Definición técnica:  
División de una red en zonas lógicas o físicas para limitar el movimiento lateral y aplicar políticas diferenciadas.

Propósito arquitectónico:  
Confinar amenazas, reducir exposición y facilitar control granular.

Integración en sistemas:  
VLAN, firewalls, ACLs, SDN y arquitecturas Zero Trust.

Aforismo:  
Lo que no se mezcla, no se contamina.

Tokenización

Definición técnica:  
Sustitución de datos sensibles por identificadores únicos sin valor intrínseco.

Propósito arquitectónico:  
Proteger información crítica sin necesidad de cifrarla directamente.

Integración en sistemas:  
Pagos, bases de datos, APIs, cumplimiento normativo y privacidad.

Aforismo:  
El símbolo viaja; el secreto permanece.

Reconocimiento pasivo

Definición técnica:  
Fase de recopilación de información sin interactuar directamente con el objetivo.

Propósito arquitectónico:  
Obtener inteligencia sin generar alertas ni dejar trazas.

Integración en sistemas:  
OSINT, análisis de DNS, metadatos, registros públicos y huellas digitales.

Aforismo:  
El que observa sin tocar, aprende sin ser visto.

Reconocimiento activo

Definición técnica:  
Fase de exploración que implica interacción directa con el objetivo para descubrir servicios, puertos y vulnerabilidades.

Propósito arquitectónico:  
Mapear la superficie expuesta y preparar fases posteriores de evaluación o ataque.

Integración en sistemas:  
Escaneo de puertos, banner grabbing, fingerprinting, traceroute y pruebas de conectividad.

Aforismo:  
Quien golpea la puerta, revela su presencia.

OSINT

Definición técnica:  
Recopilación y análisis de información pública disponible en fuentes abiertas para obtener inteligencia.

Propósito arquitectónico:  
Identificar vectores de ataque, exposición de activos y huellas digitales.

Integración en sistemas:  
Reconocimiento pasivo, análisis de amenazas, ciberinteligencia y respuesta a incidentes.

Aforismo:  
Lo que se expone sin querer, se convierte en ventaja para quien observa.

Autenticación continua

Definición técnica:  
Modelo de autenticación que evalúa de forma constante el comportamiento y el contexto del usuario para mantener o revocar el acceso.

Propósito arquitectónico:  
Reducir la dependencia de autenticaciones puntuales y detectar secuestros de sesión o cambios de riesgo en tiempo real.

Integración en sistemas:  
IAM, Zero Trust, soluciones de comportamiento del usuario (UEBA), acceso adaptativo y control contextual.

Aforismo:  
No basta con entrar; hay que seguir demostrando que eres tú.

Riesgo residual

Definición técnica:  
Nivel de riesgo que permanece después de aplicar todas las medidas de mitigación razonables.

Propósito arquitectónico:  
Determinar el umbral aceptable de exposición y priorizar recursos de protección.

Integración en sistemas:  
Análisis de riesgo, planes de continuidad, decisiones de negocio y cumplimiento normativo.

Aforismo:  
Lo que no se elimina, se asume.

Mitigación

Definición técnica:  
Conjunto de acciones destinadas a reducir la probabilidad o el impacto de una amenaza sobre un activo.

Propósito arquitectónico:  
Disminuir el riesgo sin eliminar completamente la vulnerabilidad o la amenaza.

Integración en sistemas:  
Planes de seguridad, controles técnicos, procedimientos operativos y políticas organizativas.

Aforismo:  
Si no puedes evitarlo, al menos hazlo menos dañino.

Vulnerabilidad

Definición técnica:  
Debilidad en un sistema, proceso o configuración que puede ser explotada por una amenaza.

Propósito arquitectónico:  
Identificar puntos críticos que requieren refuerzo o corrección.

Integración en sistemas:  
Gestión de parches, escáneres de vulnerabilidades, pruebas de penetración y análisis de código.

Aforismo:  
Toda grieta es una invitación si no se repara.

Vulnerabilidad

Definición técnica:  
Debilidad en un sistema, proceso o configuración que puede ser explotada por una amenaza.

Propósito arquitectónico:  
Identificar puntos críticos que requieren refuerzo o corrección.

Integración en sistemas:  
Gestión de parches, escáneres de vulnerabilidades, pruebas de penetración y análisis de código.

Aforismo:  
Toda grieta es una invitación si no se repara.

Impacto

Definición técnica:  
Consecuencia potencial de que una amenaza se materialice sobre un activo.

Propósito arquitectónico:  
Cuantificar el daño posible para priorizar controles y decisiones.

Integración en sistemas:  
Matrices de riesgo, planes de continuidad, seguros cibernéticos y métricas de seguridad.

Aforismo:  
El riesgo no asusta por su probabilidad, sino por su consecuencia.

Probabilidad

Definición técnica:  
Grado de posibilidad de que una amenaza se materialice en un contexto determinado.

Propósito arquitectónico:  
Estimar la frecuencia esperada de eventos adversos y ajustar la estrategia de defensa.

Integración en sistemas:  
Evaluaciones de riesgo, simulaciones, análisis histórico y modelos predictivos.

Aforismo:  
Lo improbable no es imposible.

Riesgo

Definición técnica:  
Combinación de la probabilidad de que ocurra un evento y su impacto sobre los activos.

Propósito arquitectónico:  
Guiar decisiones de seguridad, priorizar recursos y justificar inversiones.

Integración en sistemas:  
Gobierno de seguridad, cumplimiento, arquitectura defensiva y gestión de incidentes.

Aforismo:  
El riesgo no se elimina; se gestiona.

Autenticación

Definición técnica:  
Proceso de verificar que una entidad es quien dice ser.

Propósito arquitectónico:  
Establecer identidad antes de permitir acceso a recursos o servicios.

Integración en sistemas:  
IAM, MFA, SSO, certificados digitales, biometría y tokens.

Aforismo:  
Sin identidad, no hay confianza.

Autorización

Definición técnica:  
Proceso de determinar si una entidad autenticada tiene permiso para realizar una acción específica.

Propósito arquitectónico:  
Controlar el acceso a recursos según políticas, roles o atributos.

Integración en sistemas:  
RBAC, ABAC, políticas IAM, firewalls, aplicaciones y microservicios.

Aforismo:  
Autenticarse es entrar; autorizarse es saber hasta dónde.