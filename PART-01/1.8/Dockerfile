FROM ubuntu:20.04
WORKDIR /usr/src/app
RUN apt update && \
    apt install -y curl
COPY PART-01/1.8/curler.sh .
CMD ./curler.sh