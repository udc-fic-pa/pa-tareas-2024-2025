# Tareas para la semana del 7 de abril

Después de las clases de esta semana, habéis adquirido los conocimientos necesarios (apartados 7.1 y 7.2) para implementar la búsqueda de productos (FUNC-2). Dado que se trata de un caso de uso muy similar al de la búsqueda de productos en pa-shop, los conocimientos adquiridos en el apartado 7.2 os serán de mucha utilidad.

A continuación os comentamos algunos aspectos en los que os debéis fijar (están resueltos en pa-shop):

- `App.jsx`debe recuperar la lista de categorías del backend.
- La lista de categorías se debe cachear en el estado de Redux.
- Por cada producto que concuerde con la búsqueda, el backend devuelve, entre otras cosas, el identificador de la categoría. Sin embargo, el frontend debe mostrar para cada producto que concuerde con la búsqueda el nombre de la categoría. Para ello, el frontend debe recuperar el nombre de la categoría a partir de la lista de categorías cacheada en el estado de Redux.
- El selector de categoría en el formulario de búsqueda de productos debe recuperar las categorías del estado de Redux.
- No olvidéis enganchar el reductor del módulo que contiene los componentes de la búsqueda de productos al reductor raíz (apartado 7.1, diapositiva 10).

