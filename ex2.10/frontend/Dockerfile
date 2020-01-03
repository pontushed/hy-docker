FROM node:10
ENV API_URL=http://localhost:8000
COPY package*.json ./
WORKDIR /
RUN npm install
COPY . .
EXPOSE 5000
CMD ["npm", "start"]
