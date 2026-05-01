---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - redes
  - seguridad
  - aislamiento
  - nube-publica
  - vpc
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
Una **Virtual Private Cloud (VPC)** es un entorno de red privado y aislado de forma lógica dentro de una nube pública. Esto significa que el cliente usa infraestructura física compartida del proveedor, pero define su propio espacio de red, separado del resto de usuarios/tenants.

Una VPC permite aprovisionar recursos de red virtualizados, como **subredes**, reglas de **firewall** y controles de acceso. Con estos elementos, la empresa decide qué recursos pueden comunicarse entre sí, cuáles pueden salir a Internet y cuáles deben mantenerse privados.

La gestión de la VPC se realiza a través de **APIs** y **CLI**, lo que permite automatizar configuración y escalado. También habilita un modelo de **autoservicio**: los equipos pueden aprovisionar redes casi instantáneamente sin intervención manual de administradores.

Aunque está alojada dentro de una nube pública, funciona como una red privada para el cliente. Dentro de ella se pueden ejecutar aplicaciones, alojar sitios, almacenar datos o conectar servicios internos con mayor control de comunicación y seguridad. Además, ofrece funciones críticas como **VPN Gateways** para conectar de forma segura infraestructura on‑premise con la VPC. A nivel de rendimiento, enfoques como **Andromeda** permiten aislamiento de rendimiento y latencia para evitar que el tráfico de otros usuarios afecte las operaciones.

El aislamiento lógico permite compartir recursos “como inquilinos en un edificio”, garantizando eficiencia de costos sin sacrificar privacidad. Por último, la **traducción de direcciones de red (NAT)** es esencial para permitir que recursos en subredes privadas accedan a Internet de forma segura.

## 📌 Puntos Claves (Opcional)
- Aislamiento lógico de red dentro de nube pública.
- Control granular: subredes, firewall, rutas, accesos.
- Gestión por APIs/CLI y autoservicio.
- Conectividad segura con on‑premise (VPN) y salida controlada (NAT).

## 🔗 Connections
- [[Cloud Público]]
- [[Cloud Híbrido]]
- [[Escalamiento horizontal y vertical en el cloud]]
- [[Requerimientos No Funcionales]]