FROM mhart/alpine-node:8.9.3

ENV NODE_ENV=production

RUN adduser -ms /bin/bash newuser

USER newuser

RUN mkdir -p /home/newuser

WORKDIR /home/newuser

COPY package.json /home/newuser

RUN npm install

COPY . /chat

EXPOSE 3000

CMD ["node","server"]
