FROM node:15
WORKDIR /var/www/front
COPY package.json /var/www/front
ARG NODE_ENV

RUN npm install; 
 

COPY . /var/www/front
ENV PORT 3000
EXPOSE $PORT
#CMD ["npm", "run", "serve"]