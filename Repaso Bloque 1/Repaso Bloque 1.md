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

