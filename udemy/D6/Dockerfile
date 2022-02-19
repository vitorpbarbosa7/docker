ARG CODE_VERSION=16.04

FROM ubuntu:${CODE_VERSION}

RUN apt-get update && apt-get install nginx -y && apt-get clean && rm -rf /var/lib/apt/lists/*

# Container will be listening to this port
EXPOSE 80

CMD ["nginx","-g","daemon off;"]

