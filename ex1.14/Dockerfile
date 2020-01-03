FROM ruby:2.6.0
RUN apt-get update && apt-get install -y git nodejs
WORKDIR /root
RUN git clone https://github.com/docker-hy/rails-example-project
WORKDIR /root/rails-example-project
RUN gem install bundler:1.17.2
RUN bundle install
RUN rails db:migrate
EXPOSE 3000
CMD rails s
