🔐 Zero Trust no es un login. Es una vigilancia viva

Muchos creen que implementar Zero Trust es exigir MFA al inicio de sesión. Pero la verdadera madurez comienza cuando dejamos de confiar incluso después de autenticar.


🧠 Zero Trust aplicado a identidades dinámicas

- En un entorno Zero Trust real:

- La identidad no se valida una sola vez: se revalida constantemente.

- El acceso no es binario (permitido/denegado), sino condicional y adaptable.

- Cada acción, cada solicitud, cada cambio de contexto es una oportunidad para reevaluar la confianza.

Esto se conoce como autenticación continua (Continuous Authentication), y representa un cambio de paradigma: pasamos de confiar en el “inicio de sesión” a confiar en el comportamiento persistente.


🧩 ¿Qué señales se evalúan en tiempo real?

- Ubicación geográfica: ¿el usuario está donde suele estar?

- Dispositivo: ¿es un endpoint corporativo gestionado o un BYOD sin control?

- Hora y frecuencia: ¿es un acceso habitual o un patrón anómalo?

- Tipo de recurso: ¿está accediendo a datos sensibles o a recursos públicos?

- Comportamiento: ¿su navegación y acciones coinciden con su rol habitual?

Estas señales alimentan un motor de riesgo que decide si mantener, degradar o revocar el acceso.


🎯 Ejemplo práctico

Un analista de datos accede a un dashboard interno desde su portátil corporativo. Todo parece normal. Pero 20 minutos después:

- Cambia de país (VPN mal configurada)

- Intenta descargar 5000 registros sensibles

- Su patrón de clics no coincide con su historial

- El sistema detecta riesgo elevado y responde:

- Revoca el token de sesión

- Solicita reautenticación con MFA

- Notifica al equipo de seguridad

- Bloquea temporalmente el acceso a datos sensibles

Esto no es ciencia ficción. Es Identity Threat Detection & Response (ITDR) en acción.


🛠️ Cómo se implementa esta arquitectura

- Risk-Based Access: políticas que adaptan el acceso según el riesgo contextual.

- Continuous Evaluation: monitoreo constante del comportamiento del usuario.

- Identity Orchestration: integración de señales desde SIEM, EDR, CASB, UEBA.

- Passwordless + FIDO2: autenticación fuerte sin depender de credenciales estáticas.

- Just-In-Time Access: privilegios temporales que expiran automáticamente.

- Session Revocation APIs: capacidad de cortar sesiones activas en tiempo real.


⚠️ Advertencias

- Zero Trust ≠ MFA: el MFA es solo el umbral inicial.

- No hay confianza implícita: ni por red, ni por dispositivo, ni por ubicación.

- El riesgo es dinámico: lo que era seguro hace 5 minutos puede no serlo ahora.

- La identidad es el nuevo perímetro: y debe ser monitoreada como un sistema vivo.


