# Docker-Commands

# Docker Commands Quick Reference

Este arquivo README fornece uma referência rápida para os comandos mais comuns e úteis do Docker, ajudando na gestão de containers, imagens, volumes, redes e outros recursos do Docker.

## Docker Version

Verifique a versão do Docker instalada.

```bash
docker --version
```

## Gerenciamento de Containers

### Listar Containers

Listar todos os containers ativos.

```bash
docker ps
```

Listar todos os containers, incluindo inativos.

```bash
docker ps -a
```

### Executar Container

Executar um container a partir de uma imagem.

```bash
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

Exemplo:

```bash
docker run -d -p 80:80 --name webserver nginx
```

### Parar Container

Parar um container em execução.

```bash
docker stop CONTAINER_ID
```

### Iniciar Container

Iniciar um container parado.

```bash
docker start CONTAINER_ID
```

### Remover Container

Remover um container específico.

```bash
docker rm CONTAINER_ID
```

Remover todos os containers parados.

```bash
docker container prune
```

## Gerenciamento de Imagens

### Listar Imagens

Listar todas as imagens locais.

```bash
docker images
```

### Construir Imagem

Construir uma imagem a partir de um Dockerfile.

```bash
docker build -t TAG .
```

### Remover Imagem

Remover uma imagem local.

```bash
docker rmi IMAGE_ID
```

## Docker Compose

### Executar Docker Compose

Iniciar serviços definidos em `docker-compose.yml`.

```bash
docker-compose up
```

Iniciar em modo 'detached' (em segundo plano).

```bash
docker-compose up -d
```

### Parar Docker Compose

Parar serviços executados via Docker Compose.

```bash
docker-compose down
```

## Volumes

### Listar Volumes

Exibir todos os volumes criados.

```bash
docker volume ls
```

### Criar Volume

Criar um novo volume.

```bash
docker volume create VOLUME_NAME
```

### Remover Volume

Remover um volume específico.

```bash
docker volume rm VOLUME_NAME
```

## Redes

### Listar Redes

Listar todas as redes Docker.

```bash
docker network ls
```

### Criar Rede

Criar uma nova rede.

```bash
docker network create NETWORK_NAME
```

### Remover Rede

Remover uma rede específica.

```bash
docker network rm NETWORK_NAME
```

---
