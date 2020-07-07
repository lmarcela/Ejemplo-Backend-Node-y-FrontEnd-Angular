INSTRUCCIONES:

PARA BACKEND:

1) Dentro de la carpeta del backend, En terminal: npm install --> Esto es para descargar la carpeta node_modules, la cual no se sube a git, las dependencias se guardar en package.json y es por eso que no hace falta indicarlas
2) node index --> Para correr el proyecto, el proyecto corre en el puerto definido en el archivo .env, ej. 3000
3) npm run dev --> Para evitar pausar el servidor cada vez que hay un cambio como ocurre con node index, esto es gracias a "dev": "nodemon index.js" del archivo package.json
4) Si se ingresa a http://localhost:3000/ va a decir 'Hello from backend' de acuerdo con server>index.js, en el mismo archivo esta la logica para listar tecnologias, devolver el resultado de la busqueda por id (EJ: http://localhost:3000/api/technology/5dccb828bdd8290d4b5401d8), busqueda por name (ej: http://localhost:3000/api/technology/search/angular).

PARA FRONTEND:

