FROM node
WORKDIR /app

COPY package.json .
RUN npm install

COPY . .
EXPOSE 80

CMD ["node", "app.js"]


# docker network create app_network

# docker run 
# --name mongo_db 
# --rm 
# -d
# --network app_network
# mongo

# docker build -t backend_image .

# docker run 
# -v "/Users/dishaagarwal/Downloads/coding_projects/docker_practise/multi-01-starting-setup/backend":/app 
# -v /app/node_modules 
# -d 
# -rm
# -p 80:80
# --name backend_container 
# --network app_network 
# backend_image