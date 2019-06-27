# Docker Compose Template :whale:

### We all need more Docker in our lives, so here's a template to make composing docker-compose.yml files easier

```
version: '3.0'  # if no version is specificed then v1 is assumed. Recommend v2 minimum

services:  # containers. same as docker run
  servicename: # a friendly name. this is also DNS name inside network (simlar to --name)
    image: # Optional if you use build:
    command: # Optional, replace the default CMD specified by the image (better than using shell script)
    environment: # Optional, same as -e in docker run
    volumes: # Optional, same as -v in docker run
  servicename2:

volumes: # Optional, same as docker volume create

networks: # Optional, same as docker network create
```

Shoutout to Bret Fisher! This was directly taken from his GitHub repo on Docker which can be found [here](https://github.com/BretFisher/udemy-docker-mastery)
