FROM python:2.7-stretch
MAINTAINER thierno11 (sakoba21@gmail.com)
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv
EXPOSE 5000
ADD student_age.py /
VOLUME ["/data"]
CMD ["python", "./student_age.py"]
