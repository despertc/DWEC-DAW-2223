# Actividades Repaso Bloque 1
## Repaso B1.1 - Estilos, eventos y manipulación del DOM
Crear una página web básica, un archivo CSS con estilos predefinidos para unos id y clases que utilizaremos posteriormente y un archivo JS para realizar distintas acciones sobre elementos del HTML.

1. Crear un div, añadirle una clase predefinida en el CSS y añadirlo al body de nuestro DOM.
2. Crear un párrafo, asignándole un id y añadiéndolo al div anteriormente creado.
3. Crear un formulario con el aspecto que aparece a continuación que realizaría una búsqueda de Google. Lo insertaremos en el div y cuando se vaya a enviar el formulario, cancelaremos el funcionamiento por defecto de este, y en cambio, realizaremos la consulta a otra página de búsqueda, modificando el documento.location, con un valor por ejemplo de https://www.bing.com/search?q=texto_del_input_con_name_q

```html
<form name="busca" action="https://www.google.es/search">
    <label for="input1">Escribe una búsqueda: </label>
    <input type="text" name="q"/>
    <input type="submit" value="Enviar" />
</form>
```

4. Modificar ahora el formulario para que al introducir un texto, este se inserte en una nueva tabla a crear que tenga el siguiente aspecto:

| Valor introducido en el campo de texto |
| :------------------------------------: |
|                Texto 1                 |
|                Texto 2                 |
|                Texto 3                 |

Cada vez que hagamos doble click sobre el texto de la tabla, se deberá borrar la fila correspondiente.



## Repaso B1.2 - Mini Tienda

En este ejercicio vamos a crear una tienda básica a partir de una web vacía que contendrá una cabecera simple, un formulario de búsqueda y una zona principal donde se incluirá la información que se reciba del servidor.

El funcionamiento de la página será:

1. Al cargar la web, se verá el formulario de búsqueda y una imagen que ocupará todo el ancho de la página.
2. El formulario podrá mostrar información a partir del id del producto a buscar del producto.
3. Cuando se busque un producto se mostrará de la mejor forma posible en la zona principal, el título, la descripción, la imagen, el precio y la categoría del producto.

Para obtener los productos se hará una petición AJAX al siguiente endpoint: https://fakestoreapi.com/products/id_producto (id_producto debe ser modificado).

El objeto que devolverá será de esta forma para el ejemplo de id_producto=1:

```json
{
    "id": 1,
    "title": "Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",
    "price": 109.95,
    "description": "Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday",
    "category": "men's clothing",
    "image": "https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg",
    "rating": {
      "rate": 3.9,
      "count": 120
    }
```

EXTRA: Se puede colocar un botón que muestre todos los productos de una categoría llamando al endpoint: https://fakestoreapi.com/products/categories

Se deberá incluir cada producto en la web con el mismo formato.
