FROM node:12

RUN mkdir /app
WORKDIR /app

COPY package.json /app
COPY yarn.lock /app

RUN yarn

COPY . /app

ENV NODE_ENV=production

RUN yarn build

EXPOSE 7100

CMD ["yarn", "start"]
