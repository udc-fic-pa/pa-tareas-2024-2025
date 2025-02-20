# Tareas para la semana del 24 de febrero

Después de la clase de teoría del 19 de febrero, habéis adquirido los conocimientos necesarios (temas 2 y 3) para implementar la capa Modelo y las pruebas automatizadas de los servicios locales (capa Lógica de Negocio).

Para la semana del 24 de febrero, os aconsejamos que hagáis las siguientes tareas en la capa Modelo:

- **Tarea 1**: Implementación del caso de uso "anunciar (insertar) un producto (FUNC-1)", así como sus pruebas automatizadas.

- **Tarea 2**: Implementación del caso de uso “buscar productos (FUNC-2)”, así como sus pruebas automatizadas.

- **Tarea 3**: Implementación del caso de uso que permite recuperar todas las categorías, así como sus pruebas automatizadas. Este caso de uso es necesario para generar el desplegable de categoría en el formulario de búsqueda de productos del frontend (de forma similar a `CatalogService.findAllCategories` en pa-shop). En los commits de esta tarea podéis usar la etiqueta FUNC-2, dado que es una tarea necesaria para la implementación de FUNC-2 a nivel global (frontend y backend).

- **Tarea 4**: Implementación del caso de uso “ver la información detallada de un producto (FUNC-3)”, así como sus pruebas automatizadas.

Un aspecto que tenéis que tener en cuenta es que, a diferencia del enfoque que seguisteis en ISD, la implementación de los casos de uso en los servicios locales no deben realizar validaciones básicas de formato de datos (aquellas que en ISD originaban que se devolviese `InputValidationException`). Por ejemplo, la implementación del caso de uso "anunciar un producto" no debe verificar si el número de minutos que durará la puja es un valor mayor que cero, o si el nombre del producto es null o un String vacío. Como aprenderéis en el tema 4, este tipo de validaciones las haréis cómodamente desde la capa de servicios REST usando un enfoque declarativo basado en anotaciones. Consecuentemente, las operaciones de los servicios locales no devolverán ninguna excepción del tipo `InputValidationException`.