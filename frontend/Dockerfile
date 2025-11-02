FROM node:alpine

WORKDIR /app

EXPOSE 5173

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

CMD ["npx", "serve", "-s", "dist", "-l", "5173"]
