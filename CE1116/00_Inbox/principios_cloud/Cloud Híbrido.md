---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - modelos-de-despliegue
  - nube-hibrida
  - redes
  - portabilidad
  - orquestacion
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
La **nube híbrida** es un ecosistema tecnológico que integra de forma funcional la infraestructura privada (on‑premise) de una empresa con los servicios de una nube pública. En lugar de operar como entornos aislados, ambos se conectan para que aplicaciones, datos y cargas de trabajo puedan distribuirse dinámicamente según las necesidades de la organización.

Este modelo se apoya en conectividad avanzada, herramientas de administración unificadas, túneles de red seguros y el uso de **APIs**. Por ejemplo, una empresa puede mantener en su infraestructura privada los sistemas más sensibles o críticos, mientras utiliza la nube pública para escalar servicios, almacenar datos adicionales o ejecutar aplicaciones que requieren mayor flexibilidad.

Ofrece más flexibilidad (decidir dónde ejecutar cada sistema según costo, seguridad, rendimiento o cumplimiento), pero incrementa la complejidad de administración. La **portabilidad de aplicaciones** es un motor clave de agilidad: construir una vez y desplegar en cualquier entorno. Plataformas de orquestación como Kubernetes u OpenShift ayudan a gestionar consistencia entre entornos.

Además, la proximidad física del on‑premise o del **edge** es crítica para aplicaciones sensibles a la latencia de red hacia la nube pública. La estandarización del sistema operativo (p. ej., Linux) contribuye a que el software se comporte igual en todos los nodos. Para asegurar que el aprovisionamiento en on‑premise y nube pública sea idéntico y automatizado, se recomienda implementar **Infraestructura como Código (IaC)**.

## 📌 Puntos Claves (Opcional)
- Integra nube pública + infraestructura privada.
- Distribuye cargas según costo/seguridad/rendimiento/cumplimiento.
- Requiere conectividad segura y administración consistente.
- Portabilidad y orquestación para consistencia.
- IaC reduce diferencias manuales entre entornos.

## 🔗 Connections
- [[Cloud Público]]
- [[Virtual Private Cloud (VPC)]]
- [[IaaS vs PaaS vs SaaS]]
- [[Escalamiento horizontal y vertical en el cloud]]
- [[Requerimientos No Funcionales]]

