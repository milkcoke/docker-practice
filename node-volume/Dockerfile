FROM node:alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

# 만약에 HOST OS, Container 둘다 있으면 뭘로 설치됨?
# HOST OS 기준 우선.
COPY . .

# Don't use ENV in dockerfile when it includes private and credentials information
# because everyone can see by `docker history <image-name>`
# Use on docker run --env-file <file-name> instead of writing on Dockerfile.
ENV PORT 80

EXPOSE $PORT

VOLUME ["/temp"]

CMD [ "npm", "start" ]