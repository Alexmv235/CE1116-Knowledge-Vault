---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - modelos-de-despliegue
  - nube-publica
  - escalabilidad
  - elasticidad
  - responsabilidad-compartida
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
La **nube pública** es un modelo donde un proveedor externo ofrece recursos de cloud computing (servidores, almacenamiento, aplicaciones y otros servicios) por medio de Internet. Se denomina “pública” porque la infraestructura física es compartida por varios usuarios, pero cada cliente tiene su propio espacio separado, llamado **tenant**, donde se aíslan de forma lógica los accesos, datos, aplicaciones y servicios.

Técnicamente, la nube pública se apoya en la **virtualización** y en una arquitectura administrada por el proveedor. Mediante **hipervisores**, el proveedor divide los servidores físicos en múltiples máquinas virtuales o recursos virtualizados, asignándolos a diferentes clientes de forma controlada. También existen distintos niveles de abstracción: el usuario no administra directamente el hardware físico, sino que trabaja con recursos virtuales, plataformas o aplicaciones, según el tipo de servicio contratado.

Las **APIs** son las interfaces que permiten controlar y automatizar la gestión de recursos. Normalmente opera bajo un modelo de **pago por consumo**, lo que facilita pasar de **CapEx** (comprar infraestructura propia) a **OpEx** (pagar solo por el servicio utilizado). Además, sigue un **modelo de responsabilidad compartida**: el proveedor protege y administra la infraestructura base, mientras que el cliente debe configurar y proteger correctamente usuarios, datos, accesos y servicios.

La nube pública ofrece **elasticidad rápida**, liberando recursos automáticamente cuando la demanda disminuye para optimizar costos. Su gran ventaja es habilitar tecnología escalable sin servidores propios, evitando instalaciones internas y reduciendo la necesidad de personal especializado para administrar infraestructura física. Finalmente, la distribución global en **regiones** y **zonas de disponibilidad** permite diseñar sistemas con alta disponibilidad y resiliencia frente a fallos de infraestructura.

## 📌 Puntos Claves (Opcional)
- Infraestructura física compartida + aislamiento lógico por tenant.
- Virtualización y abstracción por capas (IaaS/PaaS/SaaS).
- Gestión por APIs y automatización.
- Pago por consumo (OpEx) vs compra de hardware (CapEx).
- Responsabilidad compartida y elasticidad.

## 🔗 Connections
- [[Virtual Private Cloud (VPC)]]
- [[Cloud Híbrido]]
- [[Escalamiento horizontal y vertical en el cloud]]
- [[IaaS vs PaaS vs SaaS]]
- [[Redundante localmente en el cloud]]
- [[Redundante en zona en el cloud]]
- [[Geo-redundante en el cloud]]
- [[Requerimientos No Funcionales]]

