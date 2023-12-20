# Proyecto de Bases de Datos y Herramientas de Administración

Este proyecto utiliza Docker Compose para orquestar varios servicios de bases de datos y herramientas de administración. Cada servicio cumple un papel específico en el manejo de bases de datos y su administración.

## Servicios

### PostgreSQL (postgres)
- **Propósito:** Servidor de base de datos PostgreSQL.
- **Puerto de Acceso:** 5432
- **Descripción:** PostgreSQL se utiliza como un sistema de gestión de bases de datos relacional. Asegúrate de configurar las variables de entorno adecuadas para el usuario, contraseña y base de datos.

### SQL Server (sqlserver)
- **Propósito:** Servidor de base de datos Microsoft SQL Server.
- **Puerto de Acceso:** 1433
- **Descripción:** SQL Server es un sistema de gestión de bases de datos relacional de Microsoft. Asegúrate de configurar la contraseña SA y montar volúmenes para persistir los datos y los secretos.

### MariaDB (mysql)
- **Propósito:** Servidor de base de datos MariaDB.
- **Puerto de Acceso:** 3306
- **Descripción:** MariaDB es un sistema de gestión de bases de datos relacional y una bifurcación de MySQL. Configura la contraseña del usuario root al iniciar el contenedor.

### MongoDB (mongo)
- **Propósito:** Servidor de base de datos MongoDB.
- **Puerto de Acceso:** Predeterminado
- **Descripción:** MongoDB es una base de datos NoSQL orientada a documentos. Asegúrate de configurar el usuario y la contraseña para la autenticación.

### MongoDB Express (mongo-express)
- **Propósito:** Interfaz web para MongoDB.
- **Puerto de Acceso:** 8081
- **Descripción:** MongoDB Express proporciona una interfaz web para gestionar bases de datos MongoDB.

### PhpMyAdmin (phpmyadmin)
- **Propósito:** Interfaz web para MariaDB.
- **Puerto de Acceso:** 8080
- **Descripción:** PhpMyAdmin es una herramienta de administración basada en web para MariaDB y MySQL.

### Adminer (adminer)
- **Propósito:** Herramienta de administración de bases de datos.
- **Puerto de Acceso:** 8080
- **Descripción:** Adminer es una herramienta de administración de bases de datos con una interfaz simple y fácil de usar.

### Pgweb (pgweb)
- **Propósito:** Cliente web para PostgreSQL.
- **Puerto de Acceso:** 8081
- **Descripción:** Pgweb proporciona una interfaz web para administrar bases de datos PostgreSQL.

### Metabase (metabase)
- **Propósito:** Plataforma de análisis y visualización de datos.
- **Puerto de Acceso:** 3000
- **Descripción:** Metabase permite realizar análisis y visualizaciones de datos de manera intuitiva. Se integra con PostgreSQL para almacenar sus datos.

## Uso

1. Asegúrate de tener Docker y Docker Compose instalados.
2. Copia el archivo `docker-compose.yml` en tu sistema.
3. Configura las variables de entorno necesarias en un archivo `.env`.
4. Ejecuta `docker-compose up -d` en el directorio con el archivo para iniciar los servicios en segundo plano.

## Notas Importantes
- Ajusta las versiones de las imágenes según tus necesidades específicas.
- Configura adecuadamente las variables de entorno y ajusta los volúmenes según sea necesario.

## Contribuciones
¡Contribuciones y mejoras son bienvenidas! Siéntete libre de enviar pull requests para mejorar este proyecto.

## Licencia
Este proyecto está bajo la [Licencia MIT](LICENSE).
