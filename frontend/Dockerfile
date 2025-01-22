FROM nginx:alpine

WORKDIR /frontend

COPY ./500.html .

COPY . .

ENTRYPOINT [”nginx”]

ENV HOST localhost:8080

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]
