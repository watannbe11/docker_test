FROM cypress/base:12.6.0
WORKDIR /app

COPY package.json .
COPY yarn.lock .

RUN yarn install
RUN yarn bin -s run cypress verify

CMD ["yarn", "cypress", "run"]