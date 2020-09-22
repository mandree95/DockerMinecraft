# PaperMC Docker Image
Forked from https://github.com/marcermarc/DockerMinecraft.

## Example Docker Compose File
```yaml
version: "3"
services:
  papermc:
    image: mandree95/papermc
    volumes:
      - ./data:/mnt/minecraft
    ports:
      - 25565:25565/tcp
      - 25565:25565/udp
    stdin_open: true
    tty: true
```