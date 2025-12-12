# 🎬 NextFilm-Back — Backend Node.js para Gestión de Stock de Películas

**NextFilm-Back** es el backend de una aplicación de gestión de inventario de películas.  
Construido con **Node.js** y **Express**, esta API REST provee los servicios necesarios para que el frontend (NextFilm-Front en Angular) pueda:

- Crear, listar, filtrar y eliminar películas  
- Gestionar stock  
- Consultar detalles de cada ítem  
- Conectarse a una base de datos real  
- Trabajar de forma robusta y estable  

Este proyecto demuestra habilidades sólidas en desarrollo backend moderno con Node.js, arquitectura modular y buenas prácticas.

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **JavaScript / TypeScript (según configuración)**
- **MongoDB / Mongoose** *(o MySQL/PostgreSQL si usas ORM tipo Sequelize o TypeORM)*
- **Dotenv**
- **JWT** (si hay autenticación)
- **Middleware personalizado**
- **Tests** con Jest / Supertest *(opcional)*

---

## 📁 Estructura del proyecto

```
nextfilm-back/
├── src/
│ ├── controllers/
│ │ └── moviesController.js
│ ├── routes/
│ │ └── moviesRoutes.js
│ ├── models/
│ │ └── movieModel.js
│ ├── services/
│ │ └── movieService.js
│ ├── config/
│ │ └── database.js
│ ├── middleware/
│ │ └── errorHandler.js
│ └── app.js
├── .env
├── package.json
└── README.md
```

> Ajusta los nombres según tu estructura real si difiere.

---

## 🚀 Instalación y ejecución

### **Requisitos**
- Node.js 16+
- Una base de datos activa (MongoDB / MySQL / PostgreSQL)

### **1. Clonar el repositorio**

git clone https://github.com/Jechig0/nextfilm-back.git
cd nextfilm-back
2. Instalar dependencias
bash
Copiar código
npm install
3. Crear archivo .env
Ejemplo básico:

env
Copiar código
PORT=3000
DB_URI=mongodb://localhost:27017/nextfilm
JWT_SECRET=un_secreto_super_seguro
4. Iniciar el servidor
bash
Copiar código
npm start
Servidor escuchando en:

bash
Copiar código
http://localhost:3000/api
🔗 Endpoints de la API
Método	Endpoint	Descripción
GET	/api/movies	Lista todas las películas
GET	/api/movies/:id	Obtiene detalles de una película
POST	/api/movies	Crea una nueva película
PUT	/api/movies/:id	Actualiza una película
DELETE	/api/movies/:id	Elimina una película
