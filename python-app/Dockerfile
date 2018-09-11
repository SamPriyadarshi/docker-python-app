FROM python:2.7-slim

WORKDIR /app
ADD . /app
ADD https://github.com/amitvashist7/docker-learner-CTS/archive/master.zip /app

RUN apt-get update
RUN apt-get install -y unzip
RUN unzip /app/master.zip

RUN pip install --trusted-host pypi.python.org -r req.txt

ENV NAME World

EXPOSE 80

CMD ["python", "/app/docker-learner-CTS-master/python-apache/app.py"]
