FROM mhart/alpine-node:8.9.3

ENV NODE_ENV=production

ENV HOME=/home/appuser

RUN mkdir $HOME/chat

COPY package.json $HOME/chat

RUN npm install

COPY . $HOME/chat

EXPOSE 3000

WORKDIR $HOME/chat

CMD ["node","server"]
