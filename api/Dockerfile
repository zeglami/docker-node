#Pull the node into our image as the initial layer 
#It will be pulled from docker hub repository or from the local computer(if we have downlaoad it )
FROM node:17-alpine

#this the work directory 
WORKDIR /app

COPY package.json .

#COPY <src> <dest> (see xNotes)
COPY . .

RUN npm install

#this app will be exposed by the container on 4000 port
EXPOSE 4000 
# required for docker desktop port mapping

CMD ["node", "app.js"]