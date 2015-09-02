# DynamoDB container for local development

## Run
```
docker run -p 8000:8000 -t rsmith/docker-nc-dynamodb
```

## Shell
Navigate to http://dockerhost:8000/shell for the dynamo gui

## Compose
```yml
dynamoDB:
  image: rsmith/docker-nc-dynamodb
  volumes:
   - .data/dynamodb/local:/var/dynamodb_local
  ports:
   - "8000:8000"
```