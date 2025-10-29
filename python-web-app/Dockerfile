FROM ubuntu
WORKDIR /app
COPY requirements.txt /app
COPY devops /app
RUN apt-get update && \
apt-get install -y python3 python3-pip && \ pip install -r requirements. txt 5& l cd devops
ENTRYPOINT ["python3"]
CMD ["manage,py", "runserver", "0.0.0.0:80"]
