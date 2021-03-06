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
| GET CONTAINER LOGS | docker logs -f <containerID> |

## Service/Microservice ecosystem default Port Mappings - (For Development purposes)
### NordStar OmniStore
| Name                                                                             | Dev Port | Docker network IP | Docker network Port |             Docker Network              |
|----------------------------------------------------------------------------------|:--------:|:-----------------:|:-------------------:|:---------------------------------------:|
| HAVE                                                                             |
| [nsoCommerceGateway](https://github.com/NordStar-OMNISTORE/nsoCommerceGateway)   |   8080   |    172.18.0.80    |        8080         | --network nso_bridge --ip=172.18.0.80   |
| [nsoAdminGateway](https://github.com/NordStar-OMNISTORE/nsoAdminGateway)         |   8081   |    172.18.0.81    |        8081         | --network nso_bridge --ip=172.18.0.81   |
| [nskPerson](https://github.com/NordStar-KINESIK/nskPerson)                       |
| [nskInventory](https://github.com/NordStar-KINESIK/nskInventory)                 |   8082   |    172.18.0.82    |        8082         | --network nso_bridge --ip=172.18.0.82   |
| [nskInvoice](https://github.com/NordStar-KINESIK/nskInvoice)                     |   8083   |    172.18.0.83    |        8083         | --network nso_bridge --ip=172.18.0.83   |
| [nsoCart](https://github.com/NordStar-KINESIK/nskCart)                           |   8084   |    172.18.0.84    |        8084         | --network nso_bridge --ip=172.18.0.84   |
| [nsoSession](https://github.com/NordStar-OMNISTORE/nsoSession)                   |   8087   |    172.18.0.87    |        8087         | --network nso_bridge --ip=172.18.0.87   |
| [nsoCatalog](https://github.com/NordStar-OMNISTORE/nsoCatalog)                   |   8085   |    172.18.0.85    |        8085         | --network nso_bridge --ip=172.18.0.85   |
| [nsoRating](https://github.com/NordStar-KINESIK/nskRating)                       |   8086   |    172.18.0.86    |        8086         | --network nso_bridge --ip=172.18.0.86   |
| [nskSales](https://github.com/NordStar-OMNISTORE/nsoSales)                       |   8092   |    172.18.0.92    |        8092         | --network nso_bridge --ip=172.18.0.92   |
| [nskClient](https://github.com/NordStar-KINESIK/nskClient)                       |   8093   |    172.18.0.93    |        8093         | --network nso_bridge --ip=172.18.0.93   |
| [nskAddress](https://github.com/NordStar-KINESIK/nskAddress)                     |   8094   |    172.18.0.94    |        8094         | --network nso_bridge --ip=172.18.0.94   |
| [junjo](https://github.com/pmarquez/junjo)                                       |   8100   |   172.18.0.100    |        8100         | --network nso_bridge --ip=172.18.0.100  |
| TO DO                                                                            |
| CommerceAccountGateway                                                           |
| nskShipping                                                                      |
| nskPayment                                                                       |
| nskImage                                                                         |
| [nsPostman](https://github.com/NordStar-KINESIK/nsPostman)                       |   8095   |
| [nsoView](https://github.com/NordStar-KINESIK/nskView)                           |   8096   |

### NordStar Manta
| Service Name | Port | 
| --------| -----|
| [nsmOperationsGateway](https://github.com/NordStar-KINESIK/nskECommGWay)         |   8080   |
| [nsmAdminGateway](https://github.com/NordStar-OMNISTORE/nsoAdminGateway)         |   8081   |
| [nsmServiceOrder](https://github.com/NordStar-MANTA/nsmServiceOrder)             |   8094   |
| [nskInventory](https://github.com/NordStar-KINESIK/nskInventory)                 |   8082   |
| [nskInvoice](https://github.com/NordStar-KINESIK/nskInvoice)                     |   8083   |
| [nsPostman](https://github.com/NordStar-KINESIK/nsPostman)                       |   8087   |
| [nskPerson](https://github.com/NordStar-KINESIK/nskPerson)                       |   8091   |
| [nsoSales](https://github.com/NordStar-OMNISTORE/nsoSales)                       |   8092   |
| [nskClient](https://github.com/NordStar-KINESIK/nskClient)                       |   8093   |

### NordStar KINESIK D??jo
| Service Name | Port | 
| --------| -----|
| [nskDojo](https://github.com/NordStar-KINESIK/nskDojo) | 8080 |
| [nskAccount](https://github.com/NordStar-KINESIK/nskAccount) | 8089 |
| [nskVenue](https://github.com/NordStar-KINESIK/nskVenue) | 8090 |
| [nskPerson](https://github.com/NordStar-KINESIK/nskPerson) | 8091 |
