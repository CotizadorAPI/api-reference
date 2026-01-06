## Cotizador API - Referencia de API

### Introducción

El repositorio tiene la finalidad de versionar la documentación del Cotizador API.
La misma incluye tanto la referencia de API como la explicación de los flujos utilizados.

### Contenido

El repositorio contiene un archivo en formato `JSON` que expresan la documentación utilizando el estándar [OpenAPI 3.0](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md).

El RAW del archivo `index.json` de la rama `master` es utilizado para generar la documentación en su [sitio web](http://cotizador.docs.aeroservices.com.ar/).

### Workflow

Utilizar ramas para publicar nuevos cambios y crear pull requests para modificar la rama `master`.

El flujo de trabajo sería el siguiente:

- Clonar proyecto.

  `git clone https://github.com/CotizadorAPI/api-reference.git`

- Actualizar repositorio local.

  `git pull origin master`

- Crear rama a partir de master para comenzar a documentar.

  `git checkout -b agencies_endpoint`

- Realizar modificaciones y commitear. Los commits deben contener un texto descriptivo en inglés.
- Publicar rama.

  `git push -u origin agencies_endpoint`

- Crear pull request para mergear contenido a `master`.

### Editor de OpenAPI 3.0

Recomendamos utilizar [Swagger Editor](https://github.com/swagger-api/swagger-editor) para editar la documentación. La edición se realiza en formato `YAML`, permite importar y exportar en los formatos solicitados (`YAML` y `JSON`) y posee un validador de sintaxis en tiempo real. En este repositorio interesa almacenar únicamente el archivo con formato `JSON`.

Para utilizar la aplicación, toda la información se puede encontrar en el [README del proyecto en GitHub](https://github.com/swagger-api/swagger-editor#swagger-editor).

