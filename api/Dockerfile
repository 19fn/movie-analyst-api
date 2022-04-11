FROM node:alpine3.15

# database 
ENV DB_HOST ${DB_HOST}
ENV DB_USER ${DB_USER}
ENV DB_PASS ${DB_PASS}
ENV DB_NAME ${DB_NAME}
ENV BACKEND_PORT ${BACKEND_PORT}

WORKDIR /moviemaker/api

COPY . .

EXPOSE 3000

RUN npm install && apk add curl

CMD [ "npm","start" ]
