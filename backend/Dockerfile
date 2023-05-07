#FROM alpine/curl as build

FROM node:alpine
WORKDIR /app

# Support curl for healthcheck
RUN apk update curl; \
    apk upgrade curl; \
    apk add curl;

# If expose as env_file
# This would be overwrited.
ENV PORT 80
EXPOSE $PORT

COPY package.json ./
RUN npm install
COPY . .

CMD ["node", "app.js"]