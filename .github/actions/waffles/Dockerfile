# Container image that runs your code
FROM python:3.11.0@sha256:b941b836b18734f4992a168b579b7c16ff4c3b544782953eeab3a590a7338765

# Copies your code file from your action repository to the filesystem path `/` of the container
RUN mkdir app
COPY . /app
WORKDIR /app

RUN pip install -r requirements.txt

ENTRYPOINT ["sh", "/app/entrypoint.sh"]
