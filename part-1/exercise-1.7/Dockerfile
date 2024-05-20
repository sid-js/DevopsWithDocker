# Start from the ubuntu
FROM ubuntu:22.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

COPY script.sh .


RUN apt-get update && apt-get install -y curl
RUN chmod +x ./script.sh


CMD ./script.sh
