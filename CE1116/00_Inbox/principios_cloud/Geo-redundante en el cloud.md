---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - almacenamiento
  - redundancia
  - disponibilidad
  - durabilidad
  - grs
  - recuperacion-de-desastres
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
El **Geo‑Redundant Storage (GRS)** es un tipo de almacenamiento redundante donde los datos se replican en una región principal y también en una región secundaria emparejada. Su funcionamiento combina redundancia local con redundancia geográfica, protegiendo la información ante fallos de hardware, de una zona o de una región completa.

Una característica importante es que la replicación hacia la región secundaria suele ser **asíncrona**: los datos no se copian al mismo tiempo, sino con un pequeño retraso. Por eso es imperativo definir el **RPO (Recovery Point Objective)**, ya que datos en tránsito no confirmados en la región secundaria podrían perderse ante un desastre total en la principal.

Normalmente, la región secundaria no se puede leer directamente hasta que ocurra una conmutación por error (**failover**). Existe una variante llamada **RA‑GRS (Read‑Access GRS)** que permite lecturas en la región secundaria sin esperar failover, mejorando la disponibilidad de lectura.

La separación física entre regiones (cientos de kilómetros) explica la asincronía debido a límites de propagación (velocidad de la luz en fibra). Además, los cargos por transferencia inter‑regional pueden impactar el OpEx. Las aplicaciones deben tolerar lecturas potencialmente obsoletas en la región secundaria por el retraso de replicación.

La replicación suele ocurrir sobre un backbone privado del proveedor, con mayor seguridad/eficiencia que la Internet pública. El **RTO (Recovery Time Objective)** puede ser de minutos a horas, dependiendo del tamaño del dataset y la capacidad de procesamiento en la región secundaria. En conjunto con balanceadores globales, se automatiza la redirección de tráfico tras el failover para minimizar el impacto en usuarios.

Se utiliza cuando se requiere protección ante desastres regionales y/o cuando la información es crítica y debe mantenerse en diferentes regiones por cumplimiento o continuidad del negocio.

## 📌 Puntos Claves (Opcional)
- Copia en región principal + región secundaria.
- Replicación asíncrona: requiere definir RPO.
- Failover para activar región secundaria (o RA‑GRS para lectura).
- Considerar costos inter‑región y consistencia eventual.

## 🔗 Connections
- [[Cloud Público]]
- [[Redundante localmente en el cloud]]
- [[Redundante en zona en el cloud]]
- [[Requerimientos No Funcionales]]
