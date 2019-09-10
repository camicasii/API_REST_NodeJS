#API Rest 
aplicacion que te permite crear notas 

#Crear una nota nueva 

Solicitus [POST] /notas
    {
        nota:{
            "title": "Mi API REST",
            "description":"Una API REST" ,
            "type": "js",
            "body": "nota NodeJs"
        }
    }
Respuesta [GET] /nota
{
    nota:{
            "id": 1,
            "title":"NodeJS",
            "description": "UNA api nodeJS",
            "type": "js",
            "body": "nota NodeJs"
        }
}


