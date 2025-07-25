FROM node:22.17.1-alpine

# Argumentos para usuário
ARG user
ARG uid

# Instala expo-cli globalmente
RUN npm install -g expo-cli

# Instala o tunnel
RUN npm install --global @expo/ngrok@^4.1.0

# Cria grupo e usuário com UID vindo do host
RUN addgroup -g ${uid} ${user} && \
    adduser -D -u ${uid} -G ${user} -s /bin/sh ${user}

# Instala dependências necessárias (alpine-friendly)
RUN apk add --no-cache bash

# Define diretório de trabalho
WORKDIR /app

# Ajusta permissões
RUN chown -R ${uid}:${uid} /app

# Troca para o usuário criado
USER ${user}
