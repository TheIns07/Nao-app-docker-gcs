# Usa la imagen base de Node.js
FROM node:14-alpine

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos del proyecto al directorio de trabajo
COPY . .

# Instala las dependencias del proyecto
RUN npm install
RUN npm run lint

# Expone el puerto 3000 (o el puerto que uses para tu aplicación React)
EXPOSE 3000

# Define el comando por defecto para iniciar la aplicación
CMD ["npm", "start"]