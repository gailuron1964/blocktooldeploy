# Readme

To start:
```
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 128992268287.dkr.ecr.us-east-1.amazonaws.com
docker-compose up -d
```

Docker compose commands:
```
docker compose restart
```

To renew certification, do this every 3 months

```
sudo certbot certonly --standalone
```

last update: 10/28/2022