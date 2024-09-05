# Backend MERN - Calendar 

Este es el backend de una aplicación de calendario construida con Node.js, Express y MongoDB. Proporciona una API RESTful para gestionar eventos de calendario tales como gestionar y agendar citas.

## Características

- Autenticación de usuarios con JWT
- CRUD de eventos de calendario
- Protección de rutas con middleware de autenticación
- Conexión a base de datos MongoDB

## Requisitos

- Node.js >= 14.x
- MongoDB

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/tu-usuario/calendar-app-backend.git
   cd calendar-app-backend

2. Instala dependedencias

    npm install

3. Configura las variables del entorno

    Crea un archivo .env en la raiz, usando como template el .env.template modificando las variables
    conforme a su configuración

4. inicia el servidor

    npm start

## Uso

 1. inicia el servidor

    npm start

2. La API estará disponible en http://localhost:4000 (en el caso de que así la hayas configurado)

## Endpoints

1. Autenticación
   POST /api/auth/new: Registro de usuario
   POST /api/auth: Inicio de sesión
   GET /api/auth/renew: Renovar token

2. Eventos
   GET /api/events: Obtener todos los eventos
   POST /api/events: Crear un nuevo evento
   PUT /api/events/:id: Actualizar un evento
   DELETE /api/events/:id: Eliminar un evento

## Estructura del proyecto: 
.
├── controllers
│   ├── auth.js
│   ├── events.js
├── database
│   └── config.js
├── helpers
│   └── jwt.js
├── middlewares
│   └── validar-jwt.js
├── models
│   ├── Evento.js
│   └── Usuario.js
├── routes
│   ├── auth.js
│   └── events.js
├── .env.template
├── .gitignore
├── index.js
├── package.json
└── README.md

