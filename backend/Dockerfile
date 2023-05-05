FROM node

WORKDIR /app

# If expose as env_file
# This would be overwrited.
ENV PORT 80
EXPOSE $PORT

COPY . .
RUN npm install

CMD ["node", "app.js"]