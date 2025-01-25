# AppSchool

## Descripción
AppSchool es un sistema diseñado para optimizar la administración y organización de escuelas pequeñas y academias, ofreciendo una solución integral que centraliza procesos académicos y administrativos. Con un enfoque en la digitalización y modernización, busca resolver problemas comunes como dispersión de información, procesos manuales y comunicación ineficiente.

---

## Estado del Proyecto
Actualmente, el proyecto se encuentra en desarrollo.

---

## Características Principales
1. **Gestión de Usuarios**: Registro y administración de estudiantes y profesores.
2. **Calificaciones y Asistencia**: Control detallado y en tiempo real.
3. **Horarios y Asignaturas**: Planificación eficiente para optimizar tiempos.
4. **Comunicación**: Chat interactivo, notificaciones en tiempo real y por correo electrónico.
5. **Generación de Reportes**: Análisis del rendimiento académico con reportes automatizados.

---

## Arquitectura y Tecnologías

### Microservicios
El sistema está diseñado como una arquitectura basada en microservicios, desplegada en AWS. Los microservicios incluyen:
- Gestión de usuarios
- Gestión de cursos
- Gestión de horarios
- Servicio de notificaciones
- Generación de reportes

### Lenguajes de Programación
- JavaScript
- Python
- Go
- Ruby
- PHP

### Bases de Datos
- PostgreSQL para datos relacionales
- DynamoDB para gestión de disponibilidad
- SQLite para tareas locales
- Redshift para análisis y reportes
- MongoDB para almacenamiento de datos no relacionales

### Servicios AWS
- **Load Balancer** para balanceo de carga
- **API Gateway** para manejo centralizado de solicitudes
- **S3** para almacenamiento de respaldos
- **Auto Scaling Group** para escalabilidad

---

## Instalación

### Prerrequisitos
- Docker y Docker Compose instalados.
- Cuenta configurada en AWS.

### Clonación del Repositorio
Clona el proyecto desde GitHub:
```bash
git clone https://github.com/gabriel9818/appSchool.git
```

### Configuración de Docker Compose
Ejecuta el siguiente comando para iniciar los microservicios (rellenar configuraciones según sea necesario):
```bash
docker-compose up -d
```

Ejemplo de un archivo `docker-compose.yml`:
```yaml
version: '3.8'
services:
  appschool-auth:
    image: appschool/auth-service
    ports:
      - "5000:5000"
    environment:
      - DATABASE_URL=postgresql://username:password@host:port/dbname

  appschool-courses:
    image: appschool/course-service
    ports:
      - "5001:5001"
```

---

## Créditos
- Gabriel Ruales
- Gabriela Tumbaco

---

## Contacto
Repositorio oficial: [GitHub](https://github.com/gabriel9818/appSchool)
