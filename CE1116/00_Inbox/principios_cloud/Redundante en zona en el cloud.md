---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - almacenamiento
  - redundancia
  - disponibilidad
  - durabilidad
  - zrs
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
El **Zone‑Redundant Storage (ZRS)** es un tipo de almacenamiento redundante donde los datos se replican en varias **zonas de disponibilidad** dentro de una misma región geográfica. Cada zona es una ubicación física independiente (energía, red y enfriamiento propios), es decir, centros de datos separados.

Su funcionamiento se basa en distribuir copias de los datos entre zonas. La replicación entre zonas suele ser **síncrona**, lo que garantiza que no haya pérdida de datos, pero impacta el tiempo de respuesta, ya que la escritura se confirma cuando los datos quedan guardados de forma segura en esas zonas. Los datos pueden permanecer accesibles aunque una zona falle.

Esta separación física añade milisegundos a cada escritura comparado con almacenamiento local. Además, para redirigir cargas durante un fallo se requiere una capa de red y orquestación (como **balanceadores** o **DNS**) que apunte a zonas sanas. También puede haber costos por tráfico de datos saliente entre zonas, afectando el gasto operativo (OpEx).

El sistema puede dividir la información en fragmentos (chunks) distribuidos para facilitar la recuperación rápida ante fallos de nodos específicos.

ZRS se ofrece para datos que necesitan protección contra fallos a nivel de centro de datos dentro de la misma región (por cumplimiento o porque no se requiere tolerancia a desastres regionales). Los niveles de durabilidad esperados suelen ser muy altos (por ejemplo, “11 nueves”).

## 📌 Puntos Claves (Opcional)
- Réplicas en varias zonas dentro de una región.
- Replicación síncrona: más resiliencia, más latencia.
- Requiere capa de red/orquestación para failover.
- Posibles costos adicionales por tráfico entre zonas.

## 🔗 Connections
- [[Cloud Público]]
- [[Redundante localmente en el cloud]]
- [[Geo-redundante en el cloud]]
- [[Requerimientos No Funcionales]]
