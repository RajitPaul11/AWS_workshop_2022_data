FROM alpine:latest

RUN apk add py3-pip
RUN pip3 install flask

WORKDIR /home

COPY app.py .

EXPOSE 80

ENTRYPOINT ["/usr/bin/flask","run"]

CMD ["--host=0.0.0.0", "--port=80"]
