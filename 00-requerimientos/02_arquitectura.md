# Arquitectura base (SBR)

## Capas
- **Presentación**: JSP + Bootstrap (vistas).
- **Controlador/Negocio**: Servlets + Servicios (lógica).
- **Persistencia**: DAO + conexión MySQL.
- **BD**: MySQL (tablas `usuarios`, `tickets`).

## Paquetes
- `com.sbr.web.controller`  → Servlets
- `com.sbr.web.service`     → Servicios (lógica)
- `com.sbr.web.dao`         → DAOs (consultas a BD)
- `com.sbr.web.model`       → Entidades (POJOs)
- `com.sbr.web.util`        → Utilidades (DB, seguridad)
- `com.sbr.web.filters`     → Filtros (AuthFilter)

## Entidades iniciales
- **Usuario**(id, nombre, email, password_hash, rol)
- **Ticket**(id, titulo, descripcion, prioridad, estado, fecha_creacion, usuario_id)

## Mapa de navegación (mínimo)
- `/login` → formulario de ingreso  
- `/dashboard` → bienvenida y accesos  
- `/tickets/list` → listar mis tickets  
- `/tickets/create` → crear ticket  
- `/tickets/view?id=...` → ver detalle y cambiar estado

## Seguridad
- Sesiones en login.
- Filtro `AuthFilter` para bloquear rutas excepto `/login` y estáticos.

## Frameworks/Librerías
- Java Servlets/JSP, Maven, Tomcat 10, MySQL, JDBC, Bootstrap.
