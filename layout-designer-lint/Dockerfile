FROM node:14.13.1-slim

ENV NODE_ENV production

WORKDIR /linter

RUN npm i -g npm-check-updates

COPY package.json .
COPY .stylelintrc.yaml .
COPY .htmlhintrc .

RUN npm install

COPY linter .

CMD ./linter
