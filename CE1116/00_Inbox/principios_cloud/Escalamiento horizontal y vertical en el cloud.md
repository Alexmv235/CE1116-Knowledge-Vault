---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - escalabilidad
  - elasticidad
  - alta-disponibilidad
  - rendimiento
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
La **escalabilidad en la nube** es la capacidad de un sistema o servicio de aumentar o disminuir recursos según la demanda. Esto permite responder a cambios en la carga sin cambiar toda la infraestructura. La escalabilidad puede aplicarse de dos formas principales:

- **Escalamiento vertical:** aumentar la capacidad de un recurso existente (por ejemplo, asignar más CPU o memoria a un servidor). Suele enfrentar un límite físico (capacidad máxima del host) y, frecuentemente, requiere reinicio (tiempo de inactividad), afectando la disponibilidad.
- **Escalamiento horizontal:** agregar más instancias/servidores para repartir la carga entre múltiples recursos, favoreciendo la alta disponibilidad.

Para que el escalamiento horizontal funcione correctamente, es esencial contar con **balanceadores de carga** que distribuyan solicitudes y diseñar aplicaciones **stateless** (sin estado) que no dependan de datos locales en una instancia específica. La nube permite adaptarse a crecimiento, picos de tráfico o cambios temporales, pagando únicamente por los recursos que se usan.

En arquitecturas modernas, la separación de **cómputo** y **almacenamiento** permite escalar estos recursos de forma independiente, optimizando eficiencia y rendimiento. Es importante distinguir entre **escalabilidad** (potencial de crecimiento) y **elasticidad** (capacidad automática de liberar recursos para optimizar costos en tiempo real).

En infraestructuras a gran escala, esta separación puede apoyarse en redes internas que desacoplan cómputo y almacenamiento (por ejemplo, redes como **Jupiter**), permitiendo escalar cada recurso de manera independiente.

Los disparadores de escalamiento basados en métricas permiten automatizar el proceso, y el modelo **FaaS (Function as a Service)** lleva esta automatización al extremo al escalar funciones instantáneamente sin intervención manual. Por último, escalar horizontalmente la capa de **datos** es un reto técnico mayor que escalar servicios stateless, por la necesidad de mantener consistencia e integridad al distribuir información entre nodos.

## 📌 Puntos Claves (Opcional)
- Vertical: simple, pero con límites y posible downtime.
- Horizontal: mejora disponibilidad; requiere balanceo y stateless.
- Elasticidad automatiza liberación de recursos.
- FaaS y auto‑scaling por métricas.
- Escalar datos es más complejo que servicios stateless.

## 🔗 Connections
- [[Cloud Público]]
- [[Cloud Híbrido]]
- [[IaaS vs PaaS vs SaaS]]
- [[Requerimientos No Funcionales]]
