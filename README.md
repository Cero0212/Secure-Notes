SecureNotes

Gestor de notas seguras con autenticación, sesiones y cifrado básico.

Descripción del Proyecto

SecureNotes es una aplicación web diseñada para almacenar notas personales de forma segura.
Incluye un backend en Node.js, una interfaz web ligera y contenedores Docker que permiten desplegar el proyecto rápidamente en cualquier entorno.

El objetivo es ofrecer un sistema sencillo, funcional y con un enfoque en buenas prácticas de seguridad.

 Características Principales

 Login con validación (usuario/contraseña)

 Manejo de sesiones seguras (JWT / Cookies)

 Creación, edición y eliminación de notas

 Base de datos SQLite integrada

 Arquitectura frontend + backend separada

 Soporte completo para Docker y Docker Compose

 Estructura clara de proyecto

 Tecnologías Utilizadas
Frontend

HTML5

CSS3

JavaScript

Backend

Node.js + Express

SQLite3

JWT (si usaste tokens)

bcrypt (si usaste hashing)

DevOps

Docker & DockerHub

GitHub (control de versiones)

 Estructura del Proyecto
SecureNotes/
│
├── backend/
│   ├── server.js
│   ├── database.js
│   ├── securenotes.sqlite
│   ├── Dockerfile
│   └── node_modules/ (ignorado)
│
├── frontend/
│   ├── index.html
│   ├── dashboard.html
│   ├── css/
│   ├── js/
│   ├── assets/
│   └── Dockerfile
│
├── .gitignore
├── docker-compose.yml
└── README.md

 Cómo Ejecutar el Proyecto Localmente
1. Clonar el repositorio
git clone https://github.com/USER/SecureNotes.git
cd SecureNotes

2. Iniciar backend
cd backend
npm install
node server.js

3. Iniciar frontend

No requiere instalación: solo abrir index.html.

 Ejecutar con Docker (Recomendado)
Build y correr contenedores
docker-compose up --build -d

Detener contenedores
docker-compose down
