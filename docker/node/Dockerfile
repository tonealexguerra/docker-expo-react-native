FROM node:22.17.1-alpine

# Instala expo-cli globalmente (opcional, se quiser usar npx também funciona)
RUN npm install -g expo-cli

# Define diretório de trabalho
WORKDIR /app

# Instala dependências necessárias (alpine-friendly)
RUN apk add --no-cache bash
