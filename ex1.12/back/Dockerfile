FROM ubuntu:16.04
WORKDIR /root
RUN apt-get update && apt-get install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker
WORKDIR /root/backend-example-docker
RUN npm install
RUN npm update
EXPOSE 8000
ENTRYPOINT ["npm"]
ENV FRONT_URL=http://localhost:5000
CMD ["start"]
