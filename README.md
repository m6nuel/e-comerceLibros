
# Backend E-Comerce libros

## versiónes necesarias son:

- __Node__: 12.18.3 o mayor
- __NPM__: 6.14.16 o mayor

## Comenzando

 1. clonar el repositorio
 2. ejecutar npm i




## PARA EL CORRECTO FUNCIONAMIENTO

crear un archivo llamado: `.env` que tenga la siguiente forma:

```env
DB_USER=usuariodepostgres
DB_PASSWORD=passwordDePostgres
DB_HOST=localhost
```

Reemplazar `usuariodepostgres` y `passwordDePostgres` con tus propias credenciales para conectarte a postgres. Este archivo va ser ignorado en la subida a github, ya que contiene información sensible (las credenciales).

Adicionalmente será necesario que creen desde psql una base de datos llamada `eclibros`


#### Tecnologías necesarias

- [ ] Express
- [ ] Sequelize - Postgres


## Reto


El reto es desarrollar un API REST con el que podamos conectar nuestro fronted. **Para esta tarea cuenta con un máximo de 48 horas.**

## Contexto

Estamos construyendo un e-commerce para la venta de libros, sin embargo no ****descartamos la posibilidad de vender otro tipo de productos en el futuro. El sistema que queremos construir debe estar en la capacidad de manejar inventario, vender, comprar, un carrito de compras, registrar usuarios, un perfil de usuarios y que los usuarios se puedan autenticar.

Tú tarea es construir los servicios que nos permita cumplir con estas funciones, nos preocupa mucho la seguridad por lo que queremos conocer que **practicas de seguridad** tuviste en cuenta durante el desarrollo.

### Requerimientos

- **Registro de usuarios**:
    - Los usuarios deben estar en la capacidad de registrarse indicando un correo electrónico, un nombre y una contraseña.
- **Autenticación de usuarios:**
    - Los usuarios podrán ingresar en su cuenta ingresando el correo y contraseña del registro.
- **Perfil de Usuarios:**
    - Los usuarios podrán agregar una dirección de residencia y una foto de perfil.
    - La dirección de residencia y foto de perfil se puede editar en cualquier momento.
- **Inventario de productos:**
    - Se debe poder agregar libros indicando el ISBN, título del libro, precio, autor, editorial y número de existencias.
    - En un futuro queremos tener más productos, pero no tenemos características especificas para esos productos, más allá del precio, código, nombre del producto y número de existencias.
    - Se debe poder actualizar las existencias de los producto ens cualquier momento.
    - Se debe poder registrar el ingreso (compra) de un producto indicando el distribuidor y la cantidad comprada.
    - Se debe poder consultar la lista de productos con sus existencias.
- **Productos**
    - El usuario debe poder agregar un producto al carrito de compras.
    - El usuario debe poder comprar un producto
        - Si no hay existencias, se le debe notificar al usuario al finalizar la compra.
    - El usuario debe poder consultar la lista de productos.
- Plus si construye el API con NodeJs.
- Se debe conectar a una base de datos. Plus si utiliza PostgreSQL y Prisma como ORM.
- Es importante que el API tenga documentación que explique como es su manejo.
- Tenga en cuenta parámetros de seguridad y documente que implementaciones de seguridad ha utilizado.

### Criterios de Evaluación

- Es importante que se preocupe por la escalabilidad, reutilización y la solidez de su solución. Suponga que otros desarrolladores trabajarán con usted eventualmente.
- Capacidad de entender un problema de negocio, indagar y plantear una solución.
- Capacidad para desarrollar una API.
- Uso de buenas practicas.
- Estilo de codificación.
- Documentación.
- Testing (Deseable).

### Entrega

- Envíenos un correo a **[ccastillo@aidforaids.org](mailto:ccastillo@aidforaids.org)** cuando inicie la prueba en donde indique que ya ha iniciado y cuanto tiempo estima le tomará realizar la prueba.
- Documente bien sus cambios y realice todas las confirmaciones atómicas que considere necesarias para que alguien pueda realizar un seguimiento de sus cambios mediante el control de versiones git. Envíe su solución a un repositorio de Github o Gitlab y envíenos un enlace.
- Cuando envíe su solución, por favor escriba cuanto tiempo le tomó resolver esta prueba. Solo tenga en cuenta el tiempo que usó para desarrollar la prueba, no incluya tiempo que no fue usado para desarrollar la prueba.
- Asegúrese de que su archivo README **indique a detalle como ejecutar su o sus proyectos** y como configurarlos para su correcto funcionamiento. Use este readme para documentar cualquier cosa que considere importante.
- Si tiene alguna duda o necesita ayuda con algo, no dude en contactarme. Mi email: **[ccastillo@aidforaids.org](mailto:ccastillo@aidforaids.org)** y mi número de celular: +573166573189

**¡Mucha suerte!**