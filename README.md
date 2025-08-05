# API de Parking

API RESTful desarrollada en Laravel para la gestión de parkings, documentada con Swagger (OpenAPI) usando el paquete L5-Swagger.

## Requisitos

- PHP >= 8.0  
- Composer  
- Laravel >= 10  
- MySQL u otro sistema de base de datos soportado por Laravel  

## Instalación

1. Clona el repositorio:


2. Instala dependencias con Composer:


3. Copia el archivo de entorno y configura tus variables:


4. Genera la key de la app y configura datos de la base de datos en `.env`:


5. Ejecuta las migraciones (y seeders si los tienes):


## Documentación de la API

La documentación está generada automáticamente con Swagger/OpenAPI. Para visualizarla, sigue estos pasos:

### Instalar L5-Swagger

Ejecuta:


### Generar la documentación

Después de anotar tus controladores:


### Visualiza la documentación

Accede desde tu navegador a:


Aquí podrás ver y probar todos los endpoints documentados e interactuar con la API.

## Endpoints principales

| Método | Endpoint            | Descripción                                 |
|--------|---------------------|---------------------------------------------|
| GET    | /parking            | Listar todos los parkings                   |
| GET    | /parking/{id}       | Mostrar parking por ID                      |
| POST   | /parking            | Crear un nuevo parking                      |
| GET    | /parkings/{closest} | Buscar parking más cercano (lat, long query)|

### Ejemplo de request para crear un parking


- Utiliza herramientas como Postman o la propia Swagger UI para probar los endpoints.

## Contribución

Si quieres mejorar el proyecto:

1. Haz un fork.  
2. Crea una nueva rama con tus cambios: `git checkout -b mi-feature`  
3. Haz commit y push.  
4. Envía un Pull Request.

## Licencia

Este proyecto está bajo la licencia MIT.

---

Si tienes dudas sobre la integración de Swagger, autenticación o nuevos endpoints, revisa el código de los controladores y la documentación en `/api/documentation`.

¡Happy coding!
