# docker-mc
To set up Minecraft servers with Docker on Linux

---

docker run -d \
-p 25575:25565 \
-v $PWD:/data #OPTIONAL, control over files  \
-e EULA=TRUE \
--name mc-server #Docker container name \
--restart unless-stopped #Automatic restart \
itzg/minecraft-server #Docker image
