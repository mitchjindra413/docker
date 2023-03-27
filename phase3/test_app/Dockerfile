# FROM ubuntu #not specific enought

# ADD . /app #use copy over add

# RUN apt-get update # combine run statements into one if possible
# RUN apt-get upgrade -y # should use base version
# RUN apt-get install -y nodejs ssh mysql # contianer should focus on one task
# RUN cd /app && npm install # use WORKDIR instead of run when chagning dirs

# CMD mysql & sshd & npm start

FROM node:10-alpine

WORKDIR /app 
COPY . /app

RUN npm install

CMD ["npm", "start"]