#Download base image ubuntu 16.04
FROM ubuntu:16.04

# Update Ubuntu Software repository
RUN apt-get update

# Install python falcon api framework
RUN apt-get install -y python-falcon 

COPY start_service.sh /start_service.sh

CMD ["./start_service.sh"]
