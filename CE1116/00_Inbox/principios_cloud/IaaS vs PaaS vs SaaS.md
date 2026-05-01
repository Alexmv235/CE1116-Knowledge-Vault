---
Fecha de creación: 2026-04-30 16:21
Fecha de Modificación: 2026-04-30 16:21
tags:
  - cloud
  - modelos-de-servicio
  - iaas
  - paas
  - saas
  - responsabilidad-compartida
Tema: Principios-Cloud
---

## 📚 Idea/Concepto 
Los modelos **IaaS**, **PaaS** y **SaaS** representan distintos niveles de servicio dentro del cloud computing. La diferencia principal entre ellos es qué tanto administra el proveedor de nube y qué tanto administra el cliente.

- **IaaS (Infraestructura como Servicio):** el proveedor entrega recursos de infraestructura, como servidores virtuales y almacenamiento. El proveedor se encarga del hardware físico, centros de datos y disponibilidad de la infraestructura; el cliente administra el sistema operativo, las aplicaciones, los datos y las configuraciones necesarias. En IaaS, el cliente también mantiene una parte importante de la seguridad (configuración de red, controles, cifrado, parches del SO, etc.).
- **PaaS (Plataforma como Servicio):** el proveedor ofrece un entorno completo para desarrollar, probar, ejecutar y desplegar aplicaciones. Incluye infraestructura, sistema operativo, bases de datos, herramientas y servicios. El cliente se enfoca principalmente en el desarrollo de la aplicación y sus datos; el proveedor administra la plataforma base, runtime y middleware.
- **SaaS (Software como Servicio):** el usuario accede a una aplicación completa por Internet. El cliente no administra servidores, sistemas operativos ni plataformas; todo queda a cargo del proveedor.

Estos modelos habilitan la transición de **CapEx** a **OpEx**, eliminando inversiones iniciales en infraestructura y permitiendo pago basado en uso real. El acceso suele ser por **autoservicio bajo demanda**, aprovisionando mediante **APIs**. Comprender el **modelo de responsabilidad compartida** es fundamental para saber quién debe parchar y asegurar los datos según el nivel de servicio contratado. Finalmente, la mayor abstracción de SaaS y PaaS tiende a facilitar un escalamiento más rápido y transparente para el negocio frente a IaaS, gracias a la elasticidad automática.

## 📌 Puntos Claves (Opcional)
- IaaS: más control, más responsabilidad del cliente.
- PaaS: enfoque en desarrollo, menos operación.
- SaaS: consumo directo de software.
- CapEx → OpEx y autoservicio.
- Responsabilidad compartida varía por modelo.

## 🔗 Connections
- [[Cloud Público]]
- [[Cloud Híbrido]]
- [[Escalamiento horizontal y vertical en el cloud]]
- [[Requerimientos No Funcionales]]
