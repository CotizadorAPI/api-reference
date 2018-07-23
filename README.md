## Cotizador API - Referencia de API

### Introducción

El repositorio tiene la finalidad de versionar la documentación del Cotizador API. 
La misma incluye tanto la referencia de API como la explicación de los flujos utilizados.

### Contenido

El repositorio contiene dos archivos que expresan la documentación utilizando el estándar [OpenAPI 3.0](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md).
Los archivos contienen la misma especificación escrita en dos formatos diferentes: `JSON` y `YAML`.

La editores suelen utilizar estos dos formatos tanto en la importación como en la exportación de datos, así que es necesario mantenerlos actualizados y sincronizados.

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
  
- Realizar modificaciones y commitear. Los commits deben tener un texto descriptivo en inglés y pueden ser múltiples commits.
- Publicar rama.

  `git push -u origin agencies_endpoint`
  
- Crear pull request para mergear contenido a `master`.
