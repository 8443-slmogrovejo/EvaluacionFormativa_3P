# EvaluacionFormativa_3P
Sebastian Mogrovejo

# API FUNCIONAMIENTO
Para acceder a la API lo conseguimos mediante la dirección: "api/tasks"
Y para su conexión a la base de datos:
server.port = 8090
spring.datasource.url = jdbc:postgresql://localhost:5432/H2

Dentro de Visual Studio Code mediante Thunder Client accedemos de la siguiente manera:
http://localhost:8090/api/tasks

# Operaciones CRUD
Todas las operaciones se realizarán con Visual Studio Code mediante Thunder Client
# Para CREATE
En el POST de Thunder Client en el BODY:
{
  "id": 1,
  "name": "Sebastian",
  "descripcion":"Analista",
  "fecha":"23/08/2023",
  "estado":"Activo"
}


# Para READ
Conectamos a la dirección mediante GET
http://localhost:8090/api/tasks

# Para UPDATE
Conectamos a la dirección mediante PUT, en el BODY:
{
  "id": 1,
  "name": "Sebastian",
  "descripcion":"Analista",
  "fecha":"23/08/2023",
  "estado":"Inactivo"
}

# Para DELETE
Conectamos a la dirección mediante DELETE especificando el ID a borrar:
http://localhost:8090/api/tasks/1

