FROM node:16

WORKDIR /app
COPY package*.json ./

# Instalar dependencias del proyecto y @expo/ngrok globalmente
RUN npm install --legacy-peer-deps \
    && npm install -g @expo/ngrok@4.1.0

# Copiar el resto del código fuente y el archivo .env
COPY . .

# Exponer los puertos que utiliza Expo
EXPOSE 19000 19001 19002 3000

# Comando de inicio de Expo
CMD ["npx", "expo", "start", "--tunnel"]
