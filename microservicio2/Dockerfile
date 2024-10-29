# 1. Especificar la imagen base
FROM node:22.9.0-alpine

# 2. Establecer el directorio de trabajo en el contenedor
WORKDIR /opt

# 3. Copiar package.json y package-lock.json
COPY package*.json ./

# 4. Instalar las dependencias
RUN npm install

# 5. Instalar Nodemon globalmente para su uso en desarrollo
RUN npm install -g nodemon

# 6. Copiar el resto del código de la aplicación
COPY . .

# 7. Exponer el puerto de la aplicación
EXPOSE 3000

# 8. Usar Nodemon como entrypoint en desarrollo
CMD ["npm", "run", "dev"]
