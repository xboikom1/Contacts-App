# Contacts App

Node.js + MongoDB backend for managing contacts. REST API with Swagger documentation.

## Main features
- Contacts CRUD operations
- User registration and JWT-based authentication
- Password hashing with bcrypt
- Request validation with Joi
- File upload for avatars (multer) and Cloudinary storage
- Email notifications (SMTP / nodemailer)
- Structured HTTP logging (pino / pino-http)
- Centralized error handling
- API documentation generation with Redocly / Swagger

## Tech stack
- Node.js
- Express.js
- MongoDB with Mongoose
- JSON Web Tokens
- bcrypt, multer, cloudinary, nodemailer, joi, pino
- Redocly / swagger-ui-express for API docs

## Environment variables
- PORT
- MONGODB_USER
- MONGODB_PASSWORD
- MONGODB_URL
- MONGODB_DB
- SMTP_HOST
- SMTP_PORT
- SMTP_USER
- SMTP_PASSWORD
- SMTP_FROM
- JWT_SECRET
- APP_DOMAIN
- CLOUD_NAME
- API_KEY
- API_SECRET

Purpose: configure server port, MongoDB connection, SMTP email, JWT secret, app domain, and Cloudinary credentials.

## Available npm scripts
- start: node ./src/index.js
- dev: nodemon src/index.js
- build: npm run build-docs
- build-docs: redocly bundle docs/openapi.yaml --ext json -o docs/swagger.json
- preview: redocly preview

## Author

Maksym Boiko <xboikom1@stuba.sk>
