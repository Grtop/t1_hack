FROM node:16

WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
RUN docker pull milvusdb/milvus:latest

EXPOSE 3000
CMD ["npm", "start"]
