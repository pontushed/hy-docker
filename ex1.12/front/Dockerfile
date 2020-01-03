FROM ubuntu:16.04
WORKDIR /root
RUN apt-get update && apt-get install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker
WORKDIR /root/frontend-example-docker
RUN npm install
RUN npm update
EXPOSE 5000
ENTRYPOINT ["npm"]
ENV API_URL=http://localhost:8000
CMD ["start"] 
