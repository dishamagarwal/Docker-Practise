FROM node
WORKDIR /app

COPY package.json .
RUN npm install

COPY . .
EXPOSE 80

CMD ["node", "app.js"]


# docker network create app_network

# docker run 
# --name mongo_db   ~name the container
# -v data:/data/db  ~make a named valume to make sure the data persists even after the db container is shut off
# --rm  ~automatically remove container on shutoff
# -d    ~detached mode
# --network app_network ~connect to a network in order to interact with other applications
# mongo ~name of the image the container is based on

# docker build -t backend_image .

# docker run 
# -v "/Users/dishaagarwal/Downloads/coding_projects/docker_practise/multi-01-starting-setup/backend":/app   ~bind mount to automatically update code in the running container
# -v /app/node_modules  ~anonomous volume to make sur the dependencies persist even when the code is updated
# -d 
# -rm
# -p 80:80  ~expose port 80
# --name backend_container 
# --network app_network 
# backend_image