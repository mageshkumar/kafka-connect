Docker Commands

1. For executing within docker container
```docker exec -it kafka-connect /bin/bash```
2. ```curl -X POST http://localhost:8083/connectors -H "Content-Type: application/json" -d @mysqlConnector.json```