FROM node:12-alpine as build

COPY . .

RUN yarn install

ENV NODE_ENV=production

RUN yarn build

EXPOSE 7000

CMD ["yarn", "start"]
