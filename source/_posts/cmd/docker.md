---
title: Docker Cmd
date: 2019-04-16 20:46:25
categories:
- cmd
tags:
- cmd
---

Swarm initialized: current node (0f59zdhky1o1dzakcku615xbo) is now a manager.

To add a worker to this swarm, run the following command:

    docker swarm join --token SWMTKN-1-3lxwzwu2q0rqcy8vdc5z3au8k4ly7z24gz2xgq4p9wkz9wzs1p-7usj2octkouy1clqc9lfshd1e 127.0.0.1:2377

To add a manager to this swarm, run 'docker swarm join-token manager' and follow the instructions.

docker build --tag newnius/docker-proxy .

## 进入容器方式

```
docker attach 44fc0f0582d9
sudo docker exec -it 775c7c9ee1e1 /bin/bash
```

docker-machine ls

docker-compose.yml