FROM mhart/alpine-node:8.9.3

ENV NODE_ENV=production

RUN mkdir -p /chat
WORKDIR /chat

COPY package.json $HOME/chat

RUN npm install

COPY . /chat

EXPOSE 3000

CMD ["node","server"]
