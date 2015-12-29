FROM node:5.3.0

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY ../../app/NodeBB/package.json /usr/src/app/
ONBUILD RUN npm install
ONBUILD COPY ../../app/NodeBB /usr/src/app

VOLUME ["/usr/src/app"]

CMD [ "node", "app.js" ]

