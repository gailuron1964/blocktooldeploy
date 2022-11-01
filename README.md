# Readme

To start:
```
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 128992268287.dkr.ecr.us-east-1.amazonaws.com

docker system prune
docker rmi 128992268287.dkr.ecr.us-east-1.amazonaws.com/blocktool:latest

docker-compose --env-file .env up -d
docker-compose --env-file mock.env up
```

Docker compose commands:
```
docker compose restart
```

To renew certification, do this every 3 months

```
sudo certbot certonly --standalone
```
