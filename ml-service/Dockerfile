FROM python:3.10-alpine

WORKDIR .

COPY ./requirements.txt ./requirements.txt

RUN apk add --no-cache gcc musl-dev linux-headers build-base
RUN pip install -U setuptools pip
RUN pip install --no-cache-dir -r ./requirements.txt

COPY . .
