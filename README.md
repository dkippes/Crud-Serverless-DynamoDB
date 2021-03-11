# Crud-Serverless-DynamoDB

## Requerimientos:

- Iniciar servidor local de Dynamo
- npx dynamodb-admin
- sls offline
- Tener una tabla creada llamada "users" como primary key "id_user"

# Rutas

### Trae todos los usuarios registrados
- http://localhost:3000/dev/users
<hr>
### Registra un usuario en la DB
- http://localhost:3000/dev/users/register
<hr>
### Login de un usuario + le genera un token que luego se puede usar en el post de welcome (usandolo como header)
- http://localhost:3000/dev/users/login
<hr>
### Welcome para el usuario que se logueo
- http://localhost:3000/dev/users/welcome
<hr>
No olvidar poner el token que se uso para loguear sino no va a poder responder este metodo
![Token](https://i.imgur.com/0vZpf9B.png)
<hr>
### Borra un usuario
- http://localhost:3000/dev/users/deleteUser
<hr>
### Actualiza la password de un usuario
- http://localhost:3000/dev/users/updateUser
