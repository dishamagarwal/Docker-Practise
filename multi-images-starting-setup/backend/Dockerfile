FROM node
WORKDIR /app

COPY package.json .
RUN npm install && npm install -g nodemon

COPY . .
EXPOSE 80

ENV MONGODB_USERNAME=disha
ENV MONGODB_PASSWORD=secret

CMD ["nodemon", "app.js"]      //~nodemon restarts the node server when any js file changes, npm syart is the command to utilize nomdemon


# docker network create app_network

# docker run 
# --name mongo_db                       ~name the container
# -v data:/data/db                      ~make a named valume to make sure the data persists even after the db container is shut off
# --rm                                  ~automatically remove container on shutoff
# -d                                    ~detached mode
# --network app_network                 ~connect to a network in order to interact with other applications
# -e MONGO_INITDB_ROOT_USERNAME=disha   ~authentication for db, you need to pass this along with the url while connect to the db in your code (check app.js for eg)
# -e MONGO_INITDB_ROOT_PASSWORD=secret
# mongo                                 ~name of the image the container is based on

# docker build -t backend_image .

# docker run 
# -v "/Users/dishaagarwal/Downloads/coding_projects/docker_practise/multi-01-starting-setup
# /backend":/app                        ~bind mount to automatically update code in the running container
# -v /app/node_modules                  ~anonymous volume to make sur the dependencies persist even when the code is updated
# -v logs:app/logs                      ~make sure the logs persist even after container is stopped
# -d 
# -rm
# -p 80:80                              ~expose port 80
# --name backend_container 
# --network app_network 
# backend_image