# Part 2

### [Exercise 2.1](exercises/2.1)
[](exercises/2.1/compose.yaml)
```console 
touch text.log
docker-compose up
```

### [](https://devopswithdocker.com/part-2/1-migrating-to-docker-compose#web-services-in-docker-compose)

### [Exercise 2.2](exercises/2.2)
[](exercises/2.2/compose.yaml)

```console 
docker compose up -d
browse http://localhost:8080/
docker compose rm
```

### [Exercise 2.3](exercises/2.3)

## Unchanged dockerfiles
[](exercises/2.3/compose.yaml)

```console 
docker compose up -d
browse http://localhost:5000/
docker compose rm
```

## Change to use docker networks
