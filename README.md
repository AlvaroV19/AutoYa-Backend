# AutoYa — Backend 

Este repositorio contiene el backend distribuido de AutoYa, un marketplace P2P multiciudad para alquiler de vehículos. Está basado en una arquitectura de microservicios con CQRS, eventos y Redis para garantizar disponibilidad consistente y un sistema de reservas resiliente.

---

## Arquitectura del Backend

- **Tecnologías principales**: Spring Boot 3
- Notificaciones
- Redis — cache + locking.
- PostgreSQL — búsqueda y persistencia.
- MinIO / S3 — almacenamiento de imágenes y documentos.
- MQTT / Events — comunicación eventual (sagas / notificaciones).
- CQRS + Redis — para disponibilidad y reservas confiables.
- SAGA — gestión transaccional distribuida de reservas/pagos.

---

## Funcionalidades del Backend

- Registro y login con roles (CLIENTE / PROPIETARIO).
- CRUD de vehículos con imágenes.
- Gestión de disponibilidad.
- Reservas con HOLD, expiración y confirmación.
- Pago simulado (MVP).
- Generación de contrato digital.
- Notificaciones a cliente y propietario.

---

## Enlaces del proyecto

- **Frontend AutoYa**: https://github.com/AlvaroV19/AutoYa-Frontend
- **Docs AutoYa**: https://github.com/AlvaroV19/AutoYa-Docs
- **Deployment AutoYa**: https://github.com/AlvaroV19/AutoYa-Deployment
