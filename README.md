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
