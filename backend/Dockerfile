###################################################
#######################WARNING#####################
# We not to use this Dockerfile in production
# This Dockerfile is only for debug purpose
###################################################

FROM python:3.10.12-alpine3.17
WORKDIR /opt/app
COPY requirements.txt .
RUN \
  pip install --upgrade pip \
  && pip install -r requirements.txt
EXPOSE 8000
ENTRYPOINT [ "python3", "main.py" ]