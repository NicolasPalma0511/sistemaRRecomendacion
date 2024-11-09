FROM node:16

WORKDIR /app
COPY package*.json ./
RUN npm install --legacy-peer-deps
COPY . .

# Exponer el puerto para Expo
EXPOSE 19000 19001 19002 3000

# Comando de inicio de Expo
CMD ["npx", "expo", "start", "--tunnel"]
