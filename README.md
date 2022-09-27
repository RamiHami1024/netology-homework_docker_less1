# Задача 1
1. docker pull busybox
2. docker run -it --name pinger busybox ping -c 7 netology.ru
3. docker ps -a 
4. docker logs pinger
5. docker start pinger
6. docker ps -a
7. docker logs -f pinger
8. 2-14
9. docker rm pinger
10. docker rmi busybox

# Задача 2
1. docker pull node:15.14-alpine
2. docker run -it --rm -e NAME=rami -e SURNAME=hami --name mynode node:alpine
3. const {NAME, SURNAME} = process.env; console.log(`Привет, ${NAME} ${SURNAME}`)
4. CTRL+C x2
5. docker images -a && docker rmi <image-id>

# Задача 3
1. docker pull node:15.14-alpine
2. docker run -it -d --name first_node -v $PWD:/var/first/data node:alpine
3. docker run -it -d --name second_node -v $PWD:/var/second/data node:alpine
4. image  3.4
5. image  3.5
6. ls var/second/data/ && cat var/second/data/test.txt && cat var/second/data/text.txt
7. docker ps && docker stop c27001cacd9c && docker stop bba02d2d5649
8. docker rm c27001cacd9c && docker rm bba02d2d5649
9. docker rmi node:alpine