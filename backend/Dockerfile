FROM node

WORKDIR /app

COPY package.json ./

RUN npm install

# If expose as env_file
# This would be overwrited.
ENV PORT 80

EXPOSE $PORT

CMD ["node", "app.js"]