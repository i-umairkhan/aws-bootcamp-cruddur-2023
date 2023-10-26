FROM node:16.18

ENV PORT=3000

WORKDIR /frontend-react-js

COPY ./package.json /frontend-react-js/

RUN npm install

COPY . .

EXPOSE ${PORT}

CMD ["npm","start"]
