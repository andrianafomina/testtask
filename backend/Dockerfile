###
#####
FROM python:3.9-alpine

USER root
######
WORKDIR /backend
######
COPY ./requirements.txt .
#####
RUN pip3 install --upgrade pip -r requirements.txt
#####
COPY . .
######

EXPOSE 5000
CMD ["python3", "app-es.py"]
