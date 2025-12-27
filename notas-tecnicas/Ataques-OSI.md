Ataques en capa OSI y contramedidas modernas

Muchos manuales hablan de ataques sin ubicar *dónde actúan en el modelo OSI*.  
Pero para un arquitecto de seguridad, saber la *capa exacta* y la *propiedad afectada* (confidencialidad, integridad, disponibilidad, autenticación, no repudio) es esencial.



 Clasificación doctrinal

  - *Capa 2 (Enlace de datos)*  
  - *Ataque:* MAC spoofing, ARP poisoning  
  - *Impacto:* Integridad y confidencialidad  
  - *Contramedida:* Port Security, Dynamic ARP Inspection, NAC

- *Capa 3 (Red)*  
  - *Ataque:* IP spoofing, DoS/DDoS  
  - *Impacto:* Disponibilidad y autenticación  
  - *Contramedida:* Firewalls con filtrado, IDS/IPS, rate limiting

- *Capa 4 (Transporte)*  
  - *Ataque:* TCP SYN flood, UDP flood  
  - *Impacto:* Disponibilidad  
  - *Contramedida:* SYN cookies, balanceadores con protección, mitigación DDoS

- *Capa 5-7 (Sesión, Presentación, Aplicación)*  
  - *Ataque:* Man-in-the-Middle (MitM), SQL Injection, XSS  
  - *Impacto:* Confidencialidad, integridad, autenticación  
  - *Contramedida:* TLS fuerte, validación de entradas, WAF, MFA

---

Ejemplo práctico

Un atacante lanza un *ARP poisoning* en la red local:  
- Redirige tráfico hacia su máquina.  
- Captura credenciales en texto plano.  
- Escala a un ataque MitM en capa 7.  

El sistema defensivo responde con:  
- *Dynamic ARP Inspection* en switches.  
- *TLS 1.3* para cifrar sesiones.  
- *Alertas en SIEM* correlacionando anomalías de tráfico.

---

Contramedida

Cada ataque debe documentarse con su *capa OSI* y la *propiedad afectada*.  
Esto convierte el glosario en un mapa vivo:  
- *Disponibilidad* → ataques de denegación de servicio.  
- *Confidencialidad* → sniffing, MitM.  
- *Integridad* → spoofing, inyección.  
- *Autenticación* → suplantación de identidad.  
- *No repudio* → manipulación de logs.

---

Analogía 

Imagina el castillo dividido en *siete murallas* (capas OSI).  
Cada ataque busca una muralla distinta:  
- En la muralla baja (capa 2), el enemigo se disfraza de aldeano (spoofing).  
- En la muralla media (capa 4), lanza piedras sin parar (flood).  
- En la muralla alta (capa 7), intenta engañar al escriba con pergaminos falsos (SQL Injection).  

La defensa debe ser *estratificada y coordinada*.

---

**Mini‑resumen pedagógico**

**Cada ataque debe ubicarse en su capa OSI y documentarse con la propiedad afectada.  
La defensa moderna es estratificada, contextual y viva.**
