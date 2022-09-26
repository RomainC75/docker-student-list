FROM python:2.7-stretch

LABEL Romain Chenard <rom.chenard@gmail.com

RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0

EXPOSE 5000

ADD student_age.json /data/

ADD student_age.py /app/
WORKDIR /app

VOLUME /data/

CMD [ "python", "./student_age.py" ]

# docker run --name simpleapi -p 5000:5000 -d simple_api