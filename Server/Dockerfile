# FROM alpine:latest
FROM ubuntu:latest
# RUN apk add --update --no-cache libsndfile1 python3 py-pip
RUN apt-get update && apt-get -y install libsndfile1 python3-pip
WORKDIR /app
# COPY requirements.txt .
COPY . .
# RUN pip install -U scikit-learn==0.24.2
RUN pip3 install -r requirements.txt
CMD ["python3", "app.py"]