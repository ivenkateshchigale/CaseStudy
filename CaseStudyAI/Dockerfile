FROM python:3.11-slim

WORKDIR /app

RUN apt-get update && \
    apt-get install -y default-jdk && \
    apt-get clean

ENV JAVA_HOME=/usr/lib/jvm/default-java

COPY . /app

RUN pip install --no-cache-dir -r requirements.txt

CMD ["python", "app.py"]