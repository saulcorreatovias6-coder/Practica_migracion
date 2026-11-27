# Anexo: Términos, Comandos y Referencias de la Práctica

**Asignatura:** Administración de Base de Datos  
**Alumno:** Saul Correa  
**Docente:** Diego Alberto Bollas Paredes  

---

## 1. Glosario de Términos y Herramientas
* **MariaDB:** Sistema de gestión de bases de datos relacional derivado de MySQL, utilizado en servidores Linux para almacenar y administrar datos estructurados.
* **Migración / Respaldo:** Proceso de copiar o trasladar bases de datos, tablas y registros para conservar su disponibilidad o llevarlos a otro entorno.
* **`unix_socket`:** Mecanismo de autenticación en MariaDB que valida la identidad del usuario del sistema operativo en conexiones locales sin depender exclusivamente de contraseña.
* **`read_only`:** Variable global del servidor que restringe operaciones de escritura según el rol y configuración del motor durante tareas de mantenimiento o revisión.
* **PDO (`PHP Data Objects`):** Extensión de PHP que ofrece una interfaz uniforme para conectarse a bases de datos y ejecutar consultas mediante `try-catch`, `exec()`, `query()` y `fetchAll(PDO::FETCH_ASSOC)`.

---

## 2. Comandos Frecuentes de Referencia
```bash
# Control del servicio en Linux
sudo su
systemctl status mariadb
systemctl start mariadb
systemctl stop mariadb

# Acceso local como root mediante unix_socket
mariadb