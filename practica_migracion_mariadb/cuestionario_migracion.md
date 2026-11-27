# Cuestionario: Migración, Respaldo y Recuperación en MariaDB

**Asignatura:** Administración de Base de Datos  
**Alumno:** Saul Correa  
**Docente:** Diego Alberto Bollas Paredes  

---

## Preguntas y Respuestas

### 1. ¿Qué implica migrar o respaldar una base de datos en MariaDB y qué precauciones deben tomarse?
Es copiar absolutamente toda la base de datos su estructura el como funciona , debemos de tener precaucion con vereficar el sisstema operativo y del mismo SGBD que puedan tener los permisos y que realmente se haya completado.


### 2. ¿Cuál es la diferencia entre baja física y baja lógica en una base de datos?
la baja fisica se eliminma de forma permanente, la baja logica mantiene el registro y solo lo puede tener ahi como activo o inactivo pero siguee ahi.

### 3. ¿Para qué sirven los archivos de registro (`log`) y el modo de solo lectura (`read_only`) durante operaciones de mantenimiento o migración?
son los que nos permitene saber que esta suciendo, podemos decir que es una bitocaora asi mismo activar el modo de solo lectura ayuda a que no existan modificaciones no deseaddo

### 4. ¿Cómo se gestiona la conexión y ejecución de sentencias desde PHP con PDO?
Se crea una instancia de `PDO` dentro de un bloque `try-catch` para capturar errores de conexión, utilizando `exec()` para sentencias que modifican datos (`INSERT`, `UPDATE`, `DELETE`) y `query()` junto con `fetchAll(PDO::FETCH_ASSOC)` para leer y recorrer registros (`SELECT`).

### 5. ¿Por qué en Ubuntu con MariaDB puede presentarse autenticación mediante `unix_socket` o restricciones de permisos al trabajar con archivos y servicios?
 la cuenta administrativa local suele usar `unix_socket`, y los directorios del sistema o del servidor web requieren los permisos adecuados para leer, escribir o administrar el servicio sin bloqueos por eso la autenticacion 
