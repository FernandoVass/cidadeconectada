FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3001

# O --host 0.0.0.0 é essencial para o Docker expor a porta corretamente
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0", "--port", "3001"]