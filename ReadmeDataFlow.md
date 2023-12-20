# Proyecto de Procesamiento de Datos y Generación de Informes

Este proyecto utiliza Docker Compose para orquestar tres servicios clave en el ecosistema de Apache: NiFi, Spark y Superset. Cada servicio cumple un papel específico en el procesamiento de datos y la generación de informes.

## Servicios

### NiFi (Apache NiFi)
- **Propósito:** Ingestión y Movimiento de Datos.
- **Puerto de Acceso:** 8080
- **Descripción:** NiFi simplifica la ingestión y el movimiento de datos entre sistemas. Configura flujos para conectar con fuentes de datos como ERP y listas de SharePoint.

### Spark (Apache Spark)
- **Propósito:** Procesamiento de Datos.
- **Puerto de Acceso:** 4040
- **Descripción:** Spark es ideal para el procesamiento de grandes volúmenes de datos. Puede ser utilizado para realizar análisis en tiempo real y por lotes. En este contexto, se utiliza para procesar y analizar datos generados por NiFi.

### Superset (Apache Superset)
- **Propósito:** Generación de Informes y Visualización.
- **Puerto de Acceso:** 8088
- **Descripción:** Superset permite la creación de visualizaciones y paneles interactivos. Se integra con Spark y otras fuentes de datos para crear informes visuales basados en los datos procesados.

## Uso

1. Asegúrate de tener Docker y Docker Compose instalados.
2. Copia el archivo docker-compose.yml en tu sistema.
3. Ejecuta `docker-compose up -d` en el directorio con el archivo para iniciar los servicios en segundo plano.

## Notas Importantes
- Ajusta las versiones de las imágenes según tus necesidades específicas.
- Considera la seguridad al gestionar contraseñas y secretos.

## Contribuciones
¡Contribuciones y mejoras son bienvenidas! Siéntete libre de enviar pull requests para mejorar este proyecto.

## Licencia
Este proyecto está bajo la [Licencia MIT](LICENSE).
