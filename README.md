# Appointment Scheduling System 📅

Sistema web desarrollado para la gestión y programación de citas. La aplicación permite a los usuarios solicitar citas en línea mientras que los administradores pueden gestionar las reservas, administrar usuarios y controlar la información del sistema desde un panel administrativo.

---

## Características

- Registro y programación de citas.
- Gestión de citas por parte del administrador.
- Panel de administración.
- Administración de usuarios.
- Consulta de detalles de cada cita.
- Interfaz responsiva.
- Persistencia de la información mediante MySQL.

---

## Tecnologías utilizadas

- PHP
- MySQL
- HTML5
- CSS3
- JavaScript
- Bootstrap
- jQuery
- AdminLTE

---

## Estructura del proyecto

```text
appointment-scheduling-system/
│
├── admin/
│   ├── appointments/
│   ├── user/
│   ├── system_info/
│   ├── inc/
│   ├── login.php
│   └── index.php
│
├── assets/
│   ├── css/
│   └── js/
│
├── classes/
│
├── config/
│
├── database/
│
├── DB/
│   └── citas.sql
│
├── uploads/
│
├── about.html
├── index.php
└── README.md
```

---

## Funcionalidades

### Usuarios

- Solicitar citas.
- Consultar información del servicio.
- Navegar por el sitio web.

### Administrador

- Inicio de sesión.
- Gestión de citas.
- Visualización del detalle de cada cita.
- Administración de usuarios.
- Configuración del sistema.

---

## Base de datos

El proyecto incluye el archivo:

```text
DB/citas.sql
```

Este archivo contiene toda la estructura de la base de datos necesaria para el funcionamiento del sistema.

Entre la información administrada se encuentran:

- Usuarios.
- Citas.
- Configuración del sistema.
- Información administrativa.

---

## Requisitos

Antes de ejecutar el proyecto es necesario contar con:

- PHP 8.x o superior.
- MySQL o MariaDB.
- Apache (XAMPP, WAMP o Laragon).

---

## Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/USUARIO/appointment-scheduling-system.git
```

### 2. Copiar el proyecto

Ubicar la carpeta dentro del directorio del servidor web.

Ejemplo para XAMPP:

```text
xampp/htdocs/
```

---

### 3. Crear la base de datos

Crear una nueva base de datos en MySQL e importar el archivo:

```text
DB/citas.sql
```

utilizando **phpMyAdmin** o la herramienta de administración de su preferencia.

---

### 4. Configurar la conexión

Modificar el archivo de configuración de la base de datos con las credenciales correspondientes.

Ejemplo:

```php
Host: localhost
Database: citas
User: root
Password:
```

---

## Ejecución

Iniciar Apache y MySQL.

Acceder desde el navegador:

```text
http://localhost/Citas-main/
```

Panel administrativo:

```text
http://localhost/Citas-main/admin/
```

---

## Arquitectura

```text
Usuario
    │
    ▼
Página Web
    │
    ▼
PHP
    │
    ▼
MySQL
    │
    ▼
Panel Administrativo
```

El sistema sigue una arquitectura cliente-servidor donde PHP gestiona la lógica del negocio y MySQL almacena toda la información relacionada con las citas y los usuarios.

---

## Organización del proyecto

| Carpeta | Descripción |
|----------|-------------|
| `admin/` | Panel de administración del sistema. |
| `appointments/` | Gestión de citas. |
| `user/` | Administración de usuarios. |
| `assets/` | Recursos CSS y JavaScript. |
| `config/` | Configuración de la aplicación. |
| `classes/` | Clases y lógica del sistema. |
| `DB/` | Script SQL de la base de datos. |
| `uploads/` | Archivos cargados por el sistema. |

---

## Despliegue

La aplicación puede desplegarse en cualquier servidor compatible con PHP y MySQL, como:

- Apache
- XAMPP
- WAMP
- Laragon
- cPanel
- Servidores Linux con LAMP

---

## Capturas

Puedes agregar imágenes del sistema en esta sección.

```text
docs/home.png

docs/login-admin.png

docs/panel-admin.png

docs/gestion-citas.png
```

---

## Autor

Desarrollado por **Jossely Elena Aguirre Acuña**.

---

## Licencia

Proyecto desarrollado con fines académicos y de aprendizaje para la implementación de un sistema web de programación de citas.
