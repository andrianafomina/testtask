###черновик
#####
FROM python:3.8-alpine
######
WORKDIR /backend
######
COPY ./requirements.txt .

#####
RUN pip3 install --upgrade pip -r requirements.txt
#####
COPY . .
######


CMD ["python3", "app-es.py"]

EXPOSE 5000
