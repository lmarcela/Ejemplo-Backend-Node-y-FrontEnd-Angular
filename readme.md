INSTRUCCIONES:

PARA BACKEND:

1) Dentro de la carpeta del backend, En terminal: npm install --> Esto es para descargar la carpeta node_modules, la cual no se sube a git, las dependencias se guardar en package.json y es por eso que no hace falta indicarlas
2) En mongoDB atlas Ir a Cluster > CONNECT > Connect your application > "Copy the string and paste in .env"; Se debe asignar un nombre de usuario de BD (usermongocnn), contraseña de usuario de BD (Us3rM0ng0CNN) y nombre de BD (db_test).
3) Establecer la url de conexión en .env MONGO_URI (La BD es db_test y el nombre de la coleccion/tabla es technologies porque el modelo es technology y por defecto se crea con el nombre del modelo en plural)
4) Para crear la informacion de technology.seed.js, En terminal: npm run seed --> (Si dice technologies Created fue exitoso, en ocasiones manda error de conexion si la ip no es aceptable desde el cluster)
2) node index --> Para correr el proyecto, el proyecto corre en el puerto definido en el archivo .env, ej. 3000
3) npm run dev --> Para evitar pausar el servidor cada vez que hay un cambio como ocurre con node index, esto es gracias a "dev": "nodemon index.js" del archivo package.json
4) Si se ingresa a http://localhost:3000/ va a decir 'Hello from backend' de acuerdo con server>index.js, en el mismo archivo esta la logica para listar tecnologias, devolver el resultado de la busqueda por id (EJ: http://localhost:3000/api/technology/5f05178184fdcd3be871981a), busqueda por name (ej: http://localhost:3000/api/technology/search/angular).

PARA FRONTEND:
1) Dentro de la carpeta del backend, En terminal: npm install --> Esto es para descargar la carpeta node_modules, la cual no se sube a git, las dependencias se guardar en package.json y es por eso que no hace falta indicarlas
2) ng serve -o --> Para correr el proyecto, el proyecto corre en el puerto definido en el archivo .env, ej. 3000
3) En el archivo environment.ts se establece la ubicacion del backend (http://localhost:3000/api)
