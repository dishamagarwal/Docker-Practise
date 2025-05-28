FROM node
WORKDIR /app

COPY package.json .
RUN npm install

COPY . .
EXPOSE 3000

CMD ["npm", "start"]

# docker build -t frontend_image .

# docker run
# --name frontend_container 
# -d
# -rm
# -it
# -p 3000:3000
# -v "/Users/dishaagarwal/Downloads/coding_projects/docker_practise/multi-01-starting-setup/frontend":/app
# -v /app/node_modules
# --network app_network
# frontend_container