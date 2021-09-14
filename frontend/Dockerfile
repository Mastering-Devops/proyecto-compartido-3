FROM node:14

WORKDIR /app

COPY . .

RUN npm install -g serve && yarn install

RUN yarn build

EXPOSE 5000 

CMD ["serve","-s","build"]

