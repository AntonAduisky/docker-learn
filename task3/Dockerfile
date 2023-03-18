FROM node:16-alpine

WORKDIR /home/ilovedocker/app

COPY  ./packages/package*.json .

RUN npm i --omit=dev

COPY ./src .

EXPOSE 3032

ENTRYPOINT ["node", "main.js"]

# docker build . -t my-task-3
# docker run -p3001:3032 my-task-3
