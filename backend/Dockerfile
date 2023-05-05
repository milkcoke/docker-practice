FROM node:alpine

WORKDIR /app

# If expose as env_file
# This would be overwrited.
ENV PORT 80
EXPOSE $PORT

COPY package.json ./
RUN npm install
COPY . .

CMD ["node", "app.js"]