# Readme

To start:
```
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 128992268287.dkr.ecr.us-east-1.amazonaws.com

docker system prune
docker rmi 128992268287.dkr.ecr.us-east-1.amazonaws.com/blocktool:latest

docker-compose -f docker-compose.yaml -f docker-compose.prod.yaml up -d

docker-compose -f docker-compose.yaml -f docker-compose.dev.yaml up
```

Docker compose commands:
```
docker-compose stop

docker compose restart
```

To renew certification, do this every 3 months

```
sudo certbot certonly --standalone
```
