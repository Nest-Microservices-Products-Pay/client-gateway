# Client Gateway

## Dev

1. Clonear repositorio
2. Instalar dependencias
3. Crear archivo `.env` basado en el `.env.template`
4. Levantar ek servidor de NATS
```
docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
```
5. Tener levantados los microservicios que se van a consumir
6. Levantar el proyecto con `npm run start:dev`



## Nast
```
docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
```

## PROD
Ejecutar el comando:
```
docker build -f .\dockerfile.prod -t client-gateway .
```
