# New-Generation-Virtualization
desafio docker &amp; docker-compose

## Dockerhub - https://hub.docker.com/repository/docker/famcsn2/myfirstapp

## Lab - Docker Essentials
### Parte 01 - Setup Inicial do Docker Engine
Rodar um container com a imagem Hello world
![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/part1.png)

### Parte 02 - Customizando Imagens com DockerFile
Imagem - https://hub.docker.com/layers/163967041/famcsn2/myfirstapp/1.0/images/sha256-636ce360e092422dc15e81a0950b92b6199f245a6a82ab0ca771aa3dca5b5db0?context=repo
![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/part2.png)

### Parte 03 - Construindo um ambiente completo através do Docker Compose
Image - https://hub.docker.com/layers/163968154/famcsn2/myfirstapp/2.0/images/sha256-bd2b5d1b1938b78a099ebf118a62bf8ac6bfc03be779dd741d73c260212bfa4a?context=repo

Sem Redis

![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/part3-0.png)

Com Redis

![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/part3-1.png)


## Lab - Docker Essentials - Desafio
### DESAFIO
Incluso no arquivo `./labdocker/Dockerfile`
Imagem - https://hub.docker.com/layers/163971258/famcsn2/myfirstapp/3.0/images/sha256-caabd2d8688c8f2981f30e8cbfa4798880420b7688468a807e575e3ec3e7f01e?context=repo
![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/desafio.png)

### Extra
<<<<<<< HEAD
Incluso no arquivo `./labdocker/docker-compose.yaml` (sobrescreve o ENV com o mesmo nome do Dockerfile)

## Lab Final - GKE env & Artifactory - Desafio
### DESAFIO
Criar ambiente GKE e artifactory ou registry seguindo as instrucoes dos cards no Trello

- App
-- file `./labdocker/app.py`
-- Modifica a app para apontar o host do redis para uma variavel de ambiente
-- file `/labdocker/Dockerfile`
-- Adiciona uma nova variavel de ambiente para acesso ao redis

- Artifactory/Registry
-- Build da imagem com a modificacao feita acima
-- Push da image para o artifactory

- GKE
- dir `./manifest`
-- Os yamls irao criar 2 deployments (consequentemente replicaset e pods)
--- 1 para app web
--- 1 para redis
-- Criar 2 services
--- 1 service para a app web com type LB
--- 1 service para o redis (nao eh necessary definir type)
-- Applicar todos os yaml files com o comando abaixo
-- `kubectl apply -f .`

evidencia - tbc
=======
Incluso no ./labdocker/docker-compose.yaml (sobrescreve o ENV com o mesmo nome do Dockerfile)
![Alt text](https://raw.githubusercontent.com/Menosse/New-Generation-Virtualization/main/img/extra.png)
>>>>>>> be5012a1526a85ede32bebda58c1333f8dab7327
