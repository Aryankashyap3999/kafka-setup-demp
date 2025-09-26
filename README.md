# kafka-setup-demp

- Clone this repository

~ Move inside the cloned directory and execute the following command (Make sure docker is running in your system)
```
docker compose up -d
```
then to access kafka terminal use this command

```
docker exec -it -w /opt/kafka/bin broker sh
```
