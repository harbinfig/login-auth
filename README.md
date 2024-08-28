# login-auth
Intro
Esta API provee login y autenticacion usando nodejs, express, mongoDB, Jsonwebtoken y bcrypt. La misma permite a los usuarios registrarse y obtener tokens para la autenticacion y acceso a rutas protegidas.

Prerequisitos
Node.js and npm (or yarn) installed
Base de datos MongoDB, para esta utilizo una en mongo Atlas, en la nube

git clone https://github.com/your-username/login-auth.git

cd login-auth-api
npm install

Crea un archivo .env y coloca las variables de entorno :

MONGODB_URI=mongodb://localhost:27017/your_database_name
JWT_SECRET=your_secret_key

Replace your_database_name and your_secret_key with your actual MongoDB database name and a secure secret key for JWTs.
Reemplaza tu conexion a la base de datos y tu clave secreta:
SECRETKEY=
DBUSER=
DBPASS=
DBMONGOPASS=
SALT=


Endpoints
User Registration
Method: POST
Endpoint: /api/users/register
Request Body:
JSON
{
  "username": "your_username",
  "email": "your_email@example.com",
  "password": "your_password"
}
