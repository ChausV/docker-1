FROM ruby
RUN apt-get update && apt-get upgrade -y && apt-get install sqlite3 nodejs -y && gem install rails
COPY ./vchaus_app/ /opt/app/
WORKDIR /opt/app/
RUN bundle install
EXPOSE 3000
CMD ["rails", "s"]