# Contacts App

Node.js + MongoDB contact-management backend project with Swagger API documentation.

## Key technologies
- Node.js
- Express.js
- MongoDB / Mongoose (Data Base)
- JSON Web Tokens (authentication)
- bcrypt (password hashing)
- multer + cloudinary (file upload/storage)
- nodemailer (email)
- Joi (validation)
- pino / pino-http (logging)
- Redocly / Swagger (API documentation)

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
