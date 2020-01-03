FROM node:10
ENV FRONT_URL=http://localhost:3000
COPY package*.json ./
WORKDIR /
RUN npm install
COPY . .
EXPOSE 8000
CMD ["npm", "start"]
