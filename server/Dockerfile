FROM hospitalrun/hospitalrun-server:1.0.0-beta

COPY . /usr/src/app
COPY conf/entrypoint.sh .
#Setup the DB with initial user
RUN chmod +x conf/initcouch.sh entrypoint.sh
COPY config-demo.js config.js

EXPOSE 3000

ENTRYPOINT ./entrypoint.sh
