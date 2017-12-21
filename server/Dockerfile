FROM mhart/alpine-node:8.9.3

ENV NODE_ENV=production

RUN addgroup -S app && adduser -S -g app app 

USER app

RUN mkdir -p /home/app

WORKDIR /home/app

COPY package.json /home/app

RUN npm install

COPY . /app

EXPOSE 3000

CMD ["node","server"]
