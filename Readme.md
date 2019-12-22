manuallly creating an image from a container 

docker commit -c 'CMD ["redis-server"]' 5fb7288a19cc


#Tag your image
 docker build -t  jtjohny/simpleweb .

 #Port Mapping
 docker run -p 5000:8080 jtjohny/simpleweb

 #Interact with container
 docker run -it jtjohny/simpleweb sh
 docker exec -it 012f3474dea5 sh