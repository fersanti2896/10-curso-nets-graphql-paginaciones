# Anylist - Seed Data

Se continua con el `Backend` de Items, ahora se crea un proceso para llenar la base de datos con información cuando se cargue el proyecto.

### Pasos para iniciar API

1. Clonar repositorio e instalar los paquetes de `Node`:
```
npm install
```
2. Renombrar el archivo `.env.template` por `.env` e inicializar las variables de entorno.
3. Montar el contenedor de `Postgres` de Docker:
```
docker-compose up -d
```
4. Iniciar proyecto con:
```
npm run start:dev
```
5. Comprobar en la `URL`:
```
http://localhost:3000/graphql
```
6. Ejecutar el `SEED` en con la `mutation` de `executeSeed`.
```
mutation Mutation {
  executeSeed
}
```