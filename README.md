# AspnetMicroservices

## docker restart

    cd "C:\Program Files\Docker\Docker"
    ./DockerCli.exe -SwitchDaemon

>   docker pull mongo

        docker run -d -p 27017:27017 --name shopping-mongo mongo
        docker run -d -p 27017:27017 --name catalogdb mongo
        docker ps
        docker logs -f shopping-mongo
        docker exec -it shopping-mongo /bin/bash

        docker exec -it catalogdb /bin/bash

>   run mongo command

        mongo
        show dbs
        use CatalogDb
        db.createCollection('Products')

        db.Products.insertMany(
            [
                {
                    "Name": "Asus Laptop",
                    "Category": "Computers",
                    "Summary":  "Summary",
                    "Description":  "Description",
                    "ImageFile":    "ImageFile",
                    "Price":    54.93
                },
                {
                    "Name": "HP Laptop",
                    "Category": "Computers",
                    "Summary":  "Summary",
                    "Description":  "Description",
                    "ImageFile":    "ImageFile",
                    "Price":    88.93                    
                }
            ]
        )

        db.Products.find({}).pretty()

        db.Products.remove({})

        show databases

        show collections


>   install-package MongoDB.Driver

        Update-Package -ProjectName Catelog.API

        mongodb://localhost:27017

        mongodb://localhost:27017

        docker-compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d

        docker-compose -f .\docker-compose.yml -f .\docker-compose.override.yml down

        docker ps

        docker stop bb24

        docker rm bb24

        docker rmi bb24

        docker ps

        docker ps -a

        docker start a141

        docker images

        docker container rm 893c

>   stop / remove all 

        docker ps -aq (list all the container)

        docker stop $(docker ps -aq)

        docker rm $(docker ps -aq)

        docker rmi $(docker images -q)


>   mongo GUI

        docker run -d -p 3000:3000 mongoclient/mongoclient

>   Redis

        docker pull redis
        docker run -d -p 6379:6379 --name aspnetrun-redis redis

        docker logs -f aspnetrun-redis

        docker exec -it aspnetrun-redis /bin/bash

        


