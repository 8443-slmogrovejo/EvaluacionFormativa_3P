# EvaluacionFormativa_3P
Sebastian Mogrovejo

# API FUNCIONAMIENTO
Para acceder a la API lo conseguimos mediante la dirección: "api/tasks"<br />
Y para su conexión a la base de datos:<br />
server.port = 8090<br />
spring.datasource.url = jdbc:postgresql://localhost:5432/H2<br />

Dentro de Visual Studio Code mediante Thunder Client accedemos de la siguiente manera:<br />
http://localhost:8090/api/tasks<br />

# Operaciones CRUD
Todas las operaciones se realizarán con Visual Studio Code mediante Thunder Client
## Para CREATE
En el POST de Thunder Client en el BODY:<br />
{<br />
  "id": 1,<br />
  "name": "Sebastian",<br />
  "descripcion":"Analista",<br />
  "fecha":"23/08/2023",<br />
  "estado":"Activo"<br />
}<br />


## Para READ
Conectamos a la dirección mediante GET<br />
http://localhost:8090/api/tasks<br />

## Para UPDATE
Conectamos a la dirección mediante PUT, en el BODY:<br />
{<br />
  "id": 1,<br />
  "name": "Sebastian",<br />
  "descripcion":"Analista",<br />
  "fecha":"23/08/2023",<br />
  "estado":"Inactivo"<br />
}<br />

## Para DELETE
Conectamos a la dirección mediante DELETE especificando el ID a borrar:<br />
http://localhost:8090/api/tasks/1

