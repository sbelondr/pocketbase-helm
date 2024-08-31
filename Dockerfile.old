FROM alpine

WORKDIR /pocketbase
RUN apk update
RUN apk add wget
RUN apk add unzip
RUN wget https://github.com/pocketbase/pocketbase/releases/download/v0.22.7/pocketbase_0.22.7_linux_amd64.zip
RUN unzip pocketbase_0.22.7_linux_amd64.zip
RUN rm pocketbase_0.22.7_linux_amd64.zip
CMD [ "/pocketbase/pocketbase", "serve" ]