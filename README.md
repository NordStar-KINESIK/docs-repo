# docs-repo
Repository for all documents of the nsKINESIK platform.

## Docker Cheatsheet

| ACTION | COMMAND |
|--------|---------|
| RUN | docker run -p 27017:27017 -d mongo ( Map container port 27017 to local port 27017 ) |
| LINUX/MacOS | docker run -p 27017:27017 -v /dockerData/mongo:/data/db -d mongo   //   Maps container directory ("/data/db") to HOST directory (/dockerData/mongo) |
| WINDOWS | docker run -p 27017:27017 -v C:/dockerData/mongo:/data/db -d mongo //   On Windows, use C:/ (Volume letter and forward slashes) |
| STOP | docker stop <containerID> |
| GET CONTAINER ID | docker ps |
| GET CONTAINER LOGS | docker logs -f b472479d559a |

## Issues
[YouTrack](https://pemarquezh.myjetbrains.com/youtrack/search/Assigned%2520to%2520me-2?q=project:%20nsStore_INVENTORY)

## Service/Microservice ecosystem default Port Mappings - (For Development purposes)
| Service Name | Port | 
| --------| -----|
| [nskInventory](https://github.com/NordStar-KINESIK/nskInventory) | 8082 |
| [nskInvoice](https://github.com/NordStar-KINESIK/nskInvoice) | 8083 |
| [nskCart](https://github.com/NordStar-KINESIK/nskCart) | 8084 |
| [nskCatalog](https://github.com/NordStar-KINESIK/nskCatalog) | 8085 |
| [nskRating](https://github.com/NordStar-KINESIK/nskRating) | 8086 |
| [nsPostman](https://github.com/NordStar-KINESIK/nsPostman) | 8087 |
