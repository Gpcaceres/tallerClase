COMANDO DE DESDCARGA DE DockerHub:

  - docker pull germancinec/categories

COMANDO PARA EJECUTAR EL CONTENEDOR DE CATEGORIAS:

  - Crea la red para conectar los contenedores:
  
    docker network create net-app

  - Ejecuta el commando para arrancar el contenedor en la red:
    
    docker run -d --name app-categorias -p 8081:8081 --network net-app -e DB_HOST=test-db germancinec/categories

DIRECCIÓN:

  - http://localhost:8081/api/categories

Nota. - debe estar en ejecución la base de datos de nombre test-db

docker pull germancinec/test-db  

docker run -d --name test-db --network net-app -p 3306:3306 germancinec/test-db  


