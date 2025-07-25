# 📦 docker-react-native

Este projeto é uma aplicação de base para criação dos containers de uma aplicação Expo-React-Native.  
Siga as instruções abaixo para executar e iniciar a aplicação localmente.

---

## 🚀 Como Executar

1. Certifique-se de ter o diretório /app, totalmente vazio

2. Agora execute a criação da imagem e suba o container:

```bash
docker compose build && docker compose up -d
```

3. Com a certeza de ter atendido o passo 1, inicie o projeto Expo-React-Native

```bash
docker compose exec expo npx expo init .
```

4. Agora iniciamos o projeto para teste. Para isso use um dispositivo móvel com o app Expo Go para leitura do qrCode.

```bash
docker compose exec expo npx expo start --tunnel
```