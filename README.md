<<<<<<< HEAD
FROM python:3.6.8
#PACOTE REQUER PYTHON 3.6.X
#user/password

ENV PYTHONDONTWRITEBYTECODE=1
#Instalando pacotes necessários
ENV PYTHONUNBUFFERED=1
RUN apt install -y git
RUN git clone https://github.com/rrmmbmg/yowsup.git .
RUN python -m pip install --upgrade pip
RUN python -m pip install -r requirements.txt
WORKDIR /app
RUN adduser -u 5678 --disabled-password --gecos "" appuser && chown -R appuser /app
USER appuser
USER root
=======
<img src="https://d33wubrfki0l68.cloudfront.net/2af9b25e6ae044d480c4de738b10f8da37ed7cb1/71f28/images/python-docker.png" />


```
For simple deploy
docker-compose -f docker-compose.yml
```
```
with debug
docker-compose -f docker-compose-debug.yml
(use: python /tmp/debugpy --wait-for-client --listen 0.0.0.0:5678 {file})
```
>>>>>>> 4c7f0b0ec206a04d45a13f716cbb544581887b25
