manuallly creating an image from a container 

docker commit -c 'CMD ["redis-server"]' 5fb7288a19cc


#Tag your image
 docker build -t  jtjohny/simpleweb .

 #Port Mapping
 docker run -p 5000:8080 jtjohny/simpleweb

 #Interact with container
 docker run -it jtjohny/simpleweb sh
 docker exec -it 012f3474dea5 sh

 #docker-compose  
 -> separate cli tool that helps in connecting containers, used to start up multiple containers at the same time, automates some of the long winded arguments we were passing to docker run
 Commands : 
    docker-compose up -d
    docker-compose down
    docker-compose up --build                  ->   rebuild with code changes
    docker-compose ps


 

