# Backend

Backend - E-commerce MERN


Descripción
Este es el backend del sistema de comercio electrónico desarrollado con la pila MERN. Proporciona una API REST que gestiona usuarios, productos, categorías, carritos y órdenes, utilizando Node.js, Express y MongoDB. Además, implementa autenticación segura mediante JSON Web Tokens (JWT).

Requisitos Previos
Node.js: Descargar aquí / https://nodejs.org/en
MongoDB: Configura una instancia local o utiliza MongoDB Atlas.
Git: Descargar aquí / https://git-scm.com/

Instalación y Configuración
Clona este repositorio:

bash
Copiar código
git clone https://github.com/tu-usuario/ecommerce-mern-backend.git  
Accede a la carpeta del proyecto:

bash
Copiar código
cd ecommerce-mern-backend  
Instala las dependencias necesarias:

bash
Copiar código
npm install  
Configura las variables de entorno:

Crea un archivo .env en la raíz del proyecto con los siguientes campos:
plaintext
Copiar código
MONGO_URI=tu_url_de_conexion_a_mongodb  
JWT_SECRET=tu_secreto_para_jwt  
PORT=5000  
Inicia el servidor:

bash
Copiar código
npm start  
El backend estará disponible en http://localhost:5000.


ecommerce-mern-backend/  
├── controllers/       # Controladores de cada entidad  
├── models/            # Modelos de datos definidos con Mongoose  
├── routes/            # Definición de rutas de la API  
├── middleware/        # Middleware para autenticación y validación  
├── config/            # Configuración de base de datos  
├── server.js          # Punto de entrada principal del servidor  
└── .env               # Variables de entorno (no incluido en el repositorio)  

Endpoints del Backend
Usuarios
POST /api/users/register: Registro de usuarios.
POST /api/users/login: Iniciar sesión con autenticación JWT.
GET /api/users/profile: Obtener el perfil del usuario autenticado.
Productos
GET /api/products: Listar todos los productos.
GET /api/products/:id: Ver detalles de un producto específico.
POST /api/products: Crear un nuevo producto (solo administradores).
PUT /api/products/:id: Actualizar información de un producto (solo administradores).
DELETE /api/products/:id: Eliminar un producto (solo administradores).
Categorías
GET /api/categories: Listar todas las categorías.
POST /api/categories: Crear una categoría (solo administradores).
DELETE /api/categories/:id: Eliminar una categoría (solo administradores).
Carrito
POST /api/cart: Añadir producto al carrito del usuario autenticado.
GET /api/cart: Ver los productos en el carrito.
DELETE /api/cart/:productId: Eliminar un producto del carrito.
Órdenes
POST /api/orders: Crear una orden con los productos del carrito.
GET /api/orders: Ver las órdenes del usuario autenticado.
GET /api/orders/:id: Ver detalles de una orden específica.
Tecnologías Utilizadas
Node.js: Entorno de ejecución para JavaScript en el servidor.
Express: Framework para crear la API REST.
MongoDB: Base de datos NoSQL para el almacenamiento de datos.
Mongoose: ODM para manejar la base de datos MongoDB.
JWT (JSON Web Tokens): Autenticación segura para los usuarios.
dotenv: Gestión de variables de entorno.
Contribución
Si deseas contribuir a este proyecto:

Haz un fork del repositorio.
Crea una nueva rama para tu funcionalidad (git checkout -b nueva-funcionalidad).
Realiza tus cambios y haz commit (git commit -m "Descripción de cambios").
Sube tus cambios a tu repositorio (git push origin nueva-funcionalidad).
Abre un Pull Request en este repositorio.


¡Con este archivo README.md, tu backend estará completamente documentado para que cualquier persona pueda entender y ejecutar tu proyecto! Si necesitas ayuda adicional con GitHub, avísame.

