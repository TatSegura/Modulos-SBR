# Alcance del desarrollo (Módulos a codificar)

Proyecto: Software de soporte remoto (SBR)  
Stack: Java (Servlets/JSP) + Maven + Tomcat 10 + MySQL + Bootstrap  

## Requisitos funcionales (mínimos)
- RF1. Login/Logout de usuarios.  
- RF2. Crear ticket (título, descripción, prioridad).  
- RF3. Listar mis tickets.  
- RF4. Ver detalle y cambiar estado (Abierto, En Progreso, Cerrado).  

## Requisitos no funcionales
- RNF1. Seguridad: sesiones y hash de contraseñas.  
- RNF2. Estructura en capas (presentación, negocio, persistencia).  
- RNF3. Nombres de paquetes claros y código limpio.  
- RNF4. Despliegue en Tomcat 10 (localhost).  

## Historias de usuario (ejemplo)
- HU1. Como usuario quiero iniciar sesión para acceder a mis tickets.  
  **Criterios:** credenciales válidas → entra al dashboard; inválidas → mensaje claro.  

- HU2. Como usuario quiero crear un ticket para reportar un problema.  
  **Criterios:** campos obligatorios, validación, confirmación de creación.  

- HU3. Como usuario quiero ver y actualizar el estado de mis tickets.  
  **Criterios:** puedo filtrar/listar; cambiar estado y ver mensaje de éxito.  

## Entregables de esta evidencia
- Código fuente (02-codigo) y compilados/artefactos.  
- Diagramas (01-diagramas).  
- Pruebas (03-pruebas) con capturas.  
- Configuración de servidor/BD (04-despliegue).  
- PDF final con todo (05-pdf).  
