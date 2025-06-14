FROM node:18-alpine

WORKDIR /app

COPY package*.json ./

RUN npm ci

COPY . .

ENV CI=true

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
