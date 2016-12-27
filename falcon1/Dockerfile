#Download base image ubuntu 16.04
FROM ubuntu:16.04

# Update Ubuntu Software repository
RUN apt-get update && \
    apt-get install -y python-pip && \
    pip install --upgrade pip

# Install required python pkgs
COPY requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

COPY start_service.sh /start_service.sh

CMD ["./start_service.sh"]
