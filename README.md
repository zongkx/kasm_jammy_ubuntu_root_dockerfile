## info
this is a simple kasmweb ubuntu jammy with sudo image 


> docker build -t ubuntu-jammy-desktop:latest . 

```yaml
version: '2.2'
services:
  # sudo docker run   -it -d --shm-size=512m -p 6901:6901 -e VNC_PW=123 kasmweb/ubuntu-jammy-desktop:1.15.0-rolling
  jammy:
    image: ubuntu-jammy-desktop:latest
    ports:
      - 6901:6901
    environment:
      - VNC_PW=123123
    privileged: true
```