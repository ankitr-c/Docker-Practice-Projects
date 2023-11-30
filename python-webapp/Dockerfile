FROM python:3-alpine3.15
# FROM python:3.12-alpine
WORKDIR /app
COPY . /app/
RUN pip install -r requirements.txt
EXPOSE 8000
CMD [ "python", "app.py" ]

# FROM alpine:3.18

# RUN apk add --update python3 py3-pip

# WORKDIR /app
# COPY . /app/
# RUN pip3 install -r requirements.txt

# EXPOSE 8000  
# CMD [ "python3", "app.py" ]
