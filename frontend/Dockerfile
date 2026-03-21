FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
CMD ["cp", "-r", "/app/build/.", "/frontend_static/"]
