---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - almacenamiento
  - redundancia
  - disponibilidad
  - durabilidad
  - lrs
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
El **Locally‑Redundant Storage (LRS)** es un tipo de almacenamiento redundante donde los datos se copian varias veces dentro de un único centro de datos o zona de disponibilidad del proveedor. Su funcionamiento se basa en **replicación local**: cuando se guarda un dato, la escritura se considera correcta solo cuando la información ya quedó almacenada en sus copias internas (persistencia síncrona).

Esto reduce el riesgo de pérdida de datos si falla un disco, un servidor o parte de la infraestructura local. Un estándar común es mantener **tres réplicas** distribuidas en racks diferentes dentro del mismo centro de datos, aumentando durabilidad frente a fallos de hardware individual (disco/nodo).

LRS suele ser más barato que otros tipos de redundancia porque no replica en regiones geográficas distintas. Sin embargo, es vulnerable a desastres a nivel de edificio: no protege ante la caída total de la zona de disponibilidad. A nivel interno, el sistema puede dividir la información en **chunks** (fragmentos) distribuidos entre máquinas para facilitar recuperación ante fallos de nodos específicos, y servicios de orquestación pueden gestionar réplicas y cifrado de forma transparente.

Servicios compartidos como **Colossus** pueden encargarse de orquestar estas réplicas y el cifrado de forma transparente para el cliente.

Esta redundancia es una base que habilita cómputo elástico y resiliente (especialmente en arquitecturas stateless), ya que el almacenamiento puede escalar de forma independiente. Se usa cuando la información puede permanecer en una sola ubicación por costo, cumplimiento o porque no es crítica ante desastres regionales.

## 📌 Puntos Claves (Opcional)
- Réplicas dentro de un mismo centro de datos.
- Escrituras síncronas aumentan durabilidad local.
- Menor costo vs redundancia multi‑zona o multi‑región.
- No protege contra caída total de la zona/edificio.

## 🔗 Connections
- [[Cloud Público]]
- [[Redundante en zona en el cloud]]
- [[Geo-redundante en el cloud]]
- [[Requerimientos No Funcionales]]