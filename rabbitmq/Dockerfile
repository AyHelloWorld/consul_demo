FROM rabbitmq:latest
RUN apt-get update -y
RUN apt-get install -y python3-pip python3-dev build-essential
COPY . /rabbitmq_config
WORKDIR /rabbitmq_config
RUN chmod 777 /rabbitmq_config
RUN pip3 install -r requirements.txt
CMD ["python3", "config.py"]
