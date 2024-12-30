# Docker & PostgreSQL - postgres y DBeaver

[Docker & PostgreSQL - postgres y DBeaver](https://www.youtube.com/watch?v=hVrKX2RtigQ)

## Listar contenedores
docker ps

## Eliminar contenedor
docker rm <id/name>

## Parar Contenedor
docker stop <id/name>

## Ejecutar contenedor PostgresSQL
docker run --name menikmati-postgres -e POSTGRES_USER=menikmati -e POSTGRES_PASSWORD=password -e POSTGRES_DB=menikmatidb -p 5432:5432 -d postgres

## Ejecutar modo interactivo
docker exec -it menikmati-postgres

## Conectar por Bash a PostgresSQL
psql -U menikmati --password --db menikmatidb

## SQL current User
SELECT current_user;