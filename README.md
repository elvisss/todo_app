# API Endpoints

## PATH: /api/todo (4)
- **GET**: Listar todos los TODOs
- **POST**: Crear un TODO

## PATH: /api/todo/<em><span style="color:orange">:todoId</span></em> (4)
- **GET**: Obtener 1 TODO
- **DELETE**: Eliminar un TODO

## PATH: /api/todo/<em><span style="color:orange">:todoId</span></em>/complete (4)
- **PUT**: Marcar un TODO como **completado**/**no completado**

### Body:
```json
{
    "completed": true / false
}
```

## PATH: /api/todo/complete (2)
- **GET**: Obtener todos los TODOs completados

## PATH: /api/todo/not_complete (2)
- **GET**: Obtener todos los TODOs no completados

## PATH: /api/todo/<em><span style="color:orange">:query</span></em> (2)
- **GET**: Filtrar TODOs por el título

<br>

## Categorías

> Agregar una tabla **Category** y relacionarla con la tabla *TODO*, por lo tanto ahora un *TODO* puede pertenecer a una *categoría*.
> 
> Campos de la categoría:
> - ID
> - Title
> 
> &nbsp;

## PATH: /api/todo/<em><span style="color:orange">:categoryId</span></em> (2)
- **GET**: Obtener todos los TODOs que pertenecen a una categoría
