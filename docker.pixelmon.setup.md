
``

(didn't really get this to work)
```bash
docker run -d -v /home/jeshua/minecraft/pixelmon-01282023:/data \
    -e TYPE=CURSEFORGE \
    -e CF_SERVER_MOD=SkyFactory_4_Server_4.1.0.zip \
    -p 25565:25565 -e EULA=TRUE --name mc itzg/minecraft-server

```

URL for modpack:
1.  https://mediafilez.forgecdn.net/files/4348/478/The+Pixelmon+Modpack+8.4.3.zip

URL for mod:
3. https://mediafilez.forgecdn.net/files/4352/452/Pixelmon-1.16.5-9.1.2-universal.jar

GitHub Repo:
https://github.com/CriticalWombat/Pixelmon-Docker

This did work.
```bash
docker run -d --name "pixelmon" -p 30050:25565/tcp -p 30050:25565/udp -v /home/jeshua/minecraft/pixelmon-01282023:/data pixelmon
```

Versions
```
Pixelmon client: 1.16.5-9.0.10
```

Start-up
```bash
sudo docker start pixelmon
```