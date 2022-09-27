# Задача 1
1. docker pull busybox
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.1.png?raw=true)
2. docker run -it --name pinger busybox ping -c 7 netology.ru
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.1.png?raw=true)
3. docker ps -a 
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.1.png?raw=true)
4. docker logs pinger
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.1.png?raw=true)
5. docker start pinger
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.2.png?raw=true)
6. docker ps -a
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.3.png?raw=true)
7. docker logs -f pinger
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.4.png?raw=true)
8. 2-14
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.5.png?raw=true)
9. docker rm pinger
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.6.png?raw=true)
10. docker rmi busybox
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/1.7.png?raw=true)

# Задача 2
1. docker pull node:15.14-alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/2.1.png?raw=true)
2. docker run -it --rm -e NAME=rami -e SURNAME=hami --name mynode node:alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/2.2.png?raw=true)
3. const {NAME, SURNAME} = process.env; console.log(`Привет, ${NAME} ${SURNAME}`)
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/2.3.png?raw=true)
4. CTRL+C x2
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/2.4.png?raw=true)
5. docker images -a && docker rmi <image-id>
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/2.5.png?raw=true)

# Задача 3
1. docker pull node:15.14-alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.1.png?raw=true)
2. docker run -it -d --name first_node -v $PWD:/var/first/data node:alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.2.png?raw=true)
3. docker run -it -d --name second_node -v $PWD:/var/second/data node:alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.3.png?raw=true)
4. image  3.4
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.4.png?raw=true)
5. image  3.5
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.5.png?raw=true)
6. ls var/second/data/ && cat var/second/data/test.txt && cat var/second/data/text.txt
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.6.png?raw=true)
7. docker ps && docker stop c27001cacd9c && docker stop bba02d2d5649
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.7.png?raw=true)
8. docker rm c27001cacd9c && docker rm bba02d2d5649
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.8.png?raw=true)
9. docker rmi node:alpine
![alt text](https://github.com/RamiHami1024/netology-homework_docker_less1/blob/main/img/3.9.png?raw=true)