FROM node:alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

# 만약에 HOST OS, Container 둘다 있으면 뭘로 설치됨?
# HOST OS 기준 우선.
COPY . .

EXPOSE 80

VOLUME ["/temp"]

CMD [ "npm", "start" ]