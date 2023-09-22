# Используем официальный образ Node.js
FROM node:14

# Устанавливаем рабочую директорию внутри контейнера
WORKDIR /app

# Копируем package.json и package-lock.json и устанавливаем зависимости
COPY package*.json ./
RUN npm install

# Копируем код сервера внутрь контейнера
COPY . .

# Определяем порт, на котором будет работать сервер
EXPOSE 3001

# Запускаем сервер
CMD ["node", "index.js"]
