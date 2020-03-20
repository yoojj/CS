# Docker


- container
    - LXC
    - Libcontainer
- docker command
- docker image
- docker container
- docker network
- docker manage data
- docker registry
    - Local Registry
    - Docker Hub
    - AWS ECR
    - GCP Container Registry
    - Azure Container Registry
    - Quay (https://quay.io/)
- Dockerfile
- Docker Compose
- Docker Swarm
- Docker Machine



```bash
# 설치
$ sudo yum install -y docker docker-registry

# 버전 확인
$ docker -v

# 도커 실행
$ sudo systemctl start docker

# 도커 재실행
$ sudo systemctl restart docker

# 도커 그룹에 계정 등록
$ usermod -aG docker 계정

# 실행 확인
$ docker run hello-world
```



[top](#)
