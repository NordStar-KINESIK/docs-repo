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

## Service/Microservice ecosystem default Port Mappings - (For Development purposes)
### NordStar OmniStore
| Service Name | Port | 
| --------| -----|
| [nsoCommerceGateway](https://github.com/NordStar-KINESIK/nskECommGWay) | 8080 |
| [nsoAdminGateway](https://github.com/NordStar-OMNISTORE/nsoAdminGateway) | 8081 |
| [nskInventory](https://github.com/NordStar-KINESIK/nskInventory) | 8082 |
| [nskInvoice](https://github.com/NordStar-KINESIK/nskInvoice) | 8083 |
| [nsPostman](https://github.com/NordStar-KINESIK/nsPostman) | 8087 |
| [nsoView](https://github.com/NordStar-KINESIK/nskView) | 8088 |
| [nsoCart](https://github.com/NordStar-KINESIK/nskCart) | 8084 |
| [nsoCatalog](https://github.com/NordStar-OMNISTORE/nsoCatalog) | 8085 |
| [nsoRating](https://github.com/NordStar-KINESIK/nskRating) | 8086 |
| [nsoSales](https://github.com/NordStar-OMNISTORE/nsoSales) | 8092 |
| [nsoClient](https://github.com/NordStar-OMNISTORE/nsoClient) | 8093 |

### NordStar KINESIK Döjo
| Service Name | Port | 
| --------| -----|
| [nskDojo](https://github.com/NordStar-KINESIK/nskDojo) | 8080 |
| [nskAccount](https://github.com/NordStar-KINESIK/nskAccount) | 8089 |
| [nskVenue](https://github.com/NordStar-KINESIK/nskVenue) | 8090 |
| [nskPerson](https://github.com/NordStar-KINESIK/nskPerson) | 8091 |
