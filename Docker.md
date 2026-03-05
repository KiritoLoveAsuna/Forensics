### Docker pull image
docker pull cryptoops.azurecr.io/fetcherapp:latest

### Run and Explore Image
docker run --rm cryptoops.azurecr.io/fetcherapp:latest

### Docker Image Environment Variable
docker exec -it <container_id> /bin/sh  
docker exec -it <container_id> env

### Docker Image History
docker history cryptoops.azurecr.io/fetcherapp:latest --no-trunc --format '{{json .}}' | ConvertFrom-Json | Format-Table -Property CreatedAt, CreatedBy, Size, Comment
