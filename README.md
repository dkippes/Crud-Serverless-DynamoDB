# Crud-Serverless-DynamoDB

## Requerimientos:

- Iniciar servidor local de Dynamo
- npx dynamodb-admin
- sls offline
- Tener una tabla creada llamada "users" como primary key "id_user"

# Rutas

### Trae todos los usuarios registrados
- http://localhost:3000/dev/users

### Registra un usuario en la DB
- http://localhost:3000/dev/users/register

### Login de un usuario + le genera un token que luego se puede usar en el post de welcome (usandolo como header)
- http://localhost:3000/dev/users/login

### Welcome para el usuario que se logueo
- http://localhost:3000/dev/users/welcome

No olvidar poner el token que se uso para loguear sino no va a poder responder este metodo
![Token](https://i.imgur.com/0vZpf9B.png)

### Borra un usuario
- http://localhost:3000/dev/users/deleteUser

### Actualiza la password de un usuario
- http://localhost:3000/dev/users/updateUser
