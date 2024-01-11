FROM node

WORKDIR /app

# copying the package.json file ensures the run command is not excecuted
# if nothing changes in the file. (docker is layered)5
COPY package.json /app

RUN npm install

COPY . .

EXPOSE 80

CMD ["node", "server.js"]