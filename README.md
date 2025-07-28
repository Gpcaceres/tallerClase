COMANDO DE DESDCARGA DE DockerHub:

docker pull germancinec/categories

COMANDO PARA EJECUTAR EL CONTENEDOR DE PRODUCTOS:

docker run -d --name app-categorias-hub -p 8081:8081 --network net-categorias -e DB_HOST=test-db germancinec/categories

DIRECCIÓN:

http://localhost:8081/api/categories


