# Urls
## Hello world:
localhost:8080
## Documentacion swagger:
localhost:8080/apidocs
# Run docker
docker run -it --rm -d -p 8080:8080 -p 1234:1234 --name web byvoxel/rpc:latest

# Descripción de la aplicación
Esta aplicación utiliza RPC (Remote Procedure Call) para permitir que un cliente ejecute procedimientos en un servidor remoto. En este caso, el cliente envía el nombre de una ciudad al servidor, y el servidor responde con un mensaje de saludo que incluye el nombre de la ciudad.

# Cómo funciona el RPC en esta aplicación
1. El cliente envía una solicitud RPC al servidor con el nombre de la ciudad.
2. El servidor recibe la solicitud y ejecuta el procedimiento `SayHello` del servicio `Greeter`.
3. El procedimiento `SayHello` genera un mensaje de saludo que incluye el nombre de la ciudad y lo devuelve al cliente.
4. El cliente recibe la respuesta y la muestra en una página web.
