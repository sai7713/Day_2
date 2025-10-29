FROM ubuntu
WORKDIR /app
COPY requirements.txt /app
COPY devops /app/devops  # Copy devops folder INTO a subdirectory of /app

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    pip install --no-cache-dir -r requirements.txt

WORKDIR /app/devops  # Set the final working directory to /app/devops

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
