MongoError: command insert requires authentication

```
mongodb:
    container_name: mongo
    build:
      context: ./mongofolder
      dockerfile: ./Dockerfile
    ports:
      - "27017:27017"
    volumes:
      - ./mongofolder/data:/data/db
    env_file:
      - .env
```
- 작동안함

```
 mongodb:
    build: ./mongofolder
    ports:
      - "${MONGO_PORT}:27017"
    volumes:
      - ./mongofolder/data:/data/db
    env_file:
      - .env
```
- 작동함

- The best explanation that I could found is explanation of docker-compose links.
  - Containers for the linked service will be reachable at a hostname identical to the alias, or the service name if no alias was specified.
  - So in order to access mongoDB container from web container you should use mongoDB as host name in web container.