FROM ubuntu

COPY requirements.txt
COPY devops

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \ 
    pip install -r requirements. txt 5& l 
    
ENTRYPOINT ["python3"]
CMD ["manage,py", "runserver", "0.0.0.0:80"]
