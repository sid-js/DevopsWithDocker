FROM node:16-alpine

WORKDIR /usr/src/app

COPY . .

ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN npm install

RUN npm install -g serve

RUN npm run build

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]