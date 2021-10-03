FROM node:16

WORKDIR /usr/src/app/todo-backend

COPY . .

RUN npm install

ENV MONGO_URL="mongodb://the_username:the_password@localhost:3456/the_database" REDIS_URL="//localhost:6378"

CMD npm start
