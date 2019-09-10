# API Rest 
Aplicacion que te permite crear notas 

## Metodos HTTP permitidos
| Método    | Descripción                               |   
|-----------|  -----------------------------------------|  
|  `GET`    |  Obtener un recurso o lista de recursos   |  
|  `POST`   |Crear un recurso                           |  
|  `PUT`    |Actualizar un recurso                      |  
|  `DELETE` |Eliminar un recurso                        |  
## Codigos de respuesta
| Método    | Descripción                                               |   
|-----------|  ---------------------------------------------------------|  
|  `200`    | Success                                                   |  
|  `201`    |Success - nuevo recurso creado.                            |  
|  `204`    | success - no hay contenido para responder                 |  
|  `400`    |Bad Request - i.e. su solicitus no se puede evaluar        |  
|  `401`    |Unauthorized - isuario no esta autorizado para este recurso|  
|  `404`    |Not Found - recursos no excedio, intente mas tarde         |  
|  `422`    |Unprocessable Entity - i.e. errores de validación          |  
|  `429`    |Limite de uso excedido, intente mas tarde                  |  
|  `500`    | Error de servidor                                         |
|  `503`    | Servidor no disponible                                    |  
## Crear una nota nueva 

### Solicitus 
    POST /notas
```js
    {
        nota:{
            "title": "Mi API REST",
            "description":"Una API REST" ,
            "type": "js",
            "body": "nota NodeJs"
        }
    }
```
### Respuesta 
```js
{
    nota:{
            "id": 1,
            "title":"NodeJS",
            "description": "UNA api nodeJS",
            "type": "js",
            "body": "nota NodeJs"
        }
}
```
## Obtener una nota
 ### Solicitus 
    GET /notas/id
### Respuesta
```js
{
    nota:{
            "id": 1,
            "title":"NodeJS",
            "description": "UNA api nodeJS",
            "type": "js",
            "body": "nota NodeJs"
        }
}
```
## Actualizar una nota
 ### Solicitus 
    PUT /nota/id
```js
{
    nota:{
            "id": 1,
            "title":"Ruby",
            "description": "UNA api nodeJS",
            "type": "Ruby",
            "body": "nota Ruby"
        }
}
```
### Respuesta
```js
{
    nota:{
            "id": 1,
            "title":"Ruby",
            "description": "UNA api nodeJS",
            "type": "Ruby",
            "body": "nota Ruby"
        }
}
```
## Eliminar una nota
 ### Solicitus 
    DELETE /nota/id
### Respuesta
`200`    

