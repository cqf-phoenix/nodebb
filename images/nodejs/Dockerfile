FROM node:5.3.0

RUN mkdir -p /usr/src/app/NodeBB

WORKDIR /usr/src/app/NodeBB

ONBUILD COPY ../../app/NodeBB/package.json /usr/src/app/NodeBB
ONBUILD RUN npm install
ONBUILD COPY ../../app/NodeBB /usr/src/app/NodeBB

VOLUME ["/usr/src/app/NodeBB"]

CMD [ "./nodebb", "dev" ]


