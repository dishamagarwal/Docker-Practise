FROM node
WORKDIR /web_app
RUN npm install node
COPY . /web_app
EXPOSE 3000
CMD ["node", "server.js"]

# docker run -p 8080:3000 --rm -d --name web node