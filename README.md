# docker-mc
To set up Minecraft servers with Docker

---

docker run -d \
-p 25575:25565 \
-v $PWD:/minecraft #OPTIONAL, control over files  \
--name mc-server #Docker container name\
--restart unless-stopped #Automatic restart\
itzg/minecraft-server #Docker image
