## URL

La practica configuración de servidores está desplegada en la siguiente url:
http://ec2-44-206-49-29.compute-1.amazonaws.com/   en esta está la de node( que no funciona)
http://44.206.49.29 en esta está desplegada la de react



## EXPRESS

Se genera la app con express

npx express-generator --ejs nodepop(o como quieres que se llame la app)

Para acceder y usar la base de datos (en este caso MongoDB) ejecutar:

npm install mongoose

# Nodepop

Para arrancar la app usar:

```sh
npm install
```
En producción:

```sh
npm start
```

En desarrollo:

```sh
npm run dev
```

## Métodos del API

El api se accede en: /api

Lista de productos:

- /api/productos

Filtros:

Para filtrar por tags:

http://localhost:3000/api/productos/?sort=work

Para filtrar por tipo de anuncio(venta o busqueda):

http://localhost:3000/api/productos/?sort=venta

Para filtrar siempre utilizamos el metodo sort:

http://localhost:3000/api/productos/?sort=aquiloquequierasbuscar

Crear un producto nuevo:

-POST /api/productos

Eliminar un producto:

-DELETE /api/productos/:id


## Inicializar la BD

Para inicializar la BD al estado inicial, se puede usar el comando:
 
```sh
npm run initdb
```

* ATENCION * Esto borrará todos los datos de la BD y cargará el estado inicial.


## Rutas del api:

http://localhost:3000/api/productos

Devolverá un JSON ya sea en el navegador o en PosstMan(aqui se pueden hacer las demás peticiones:GET, POST, PUT, DELETE...)

## Ruta del frontdent

http://localhost:3000/

Renderiza y muestra los productos en un sitio web

