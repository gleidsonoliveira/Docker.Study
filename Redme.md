Docker
```
https://www.docker.com/
```

Hub docker
```
https://hub.docker.com/
```
Comandos docker 
```
https://stack.desenvolvedor.expert/appendix/docker/comandos.html
```

Verificar a versão do docker
```
 docker version
```
Comando para realizar o download da imagem para máquina local.
```
docker pull image "Nome da imagem do docker hub"
```

Comando para listar todas as imagens do docker.
```
docker image ls
```
Comando para listar os container.<br/>
Obs: Somente é necessario verificar os container em execução.
```
docker ps 
```  

Obs: Exibe os container que executaram e finalizaram por algum motivo.
``` 
docker ps -a 
```

Comando para iniciar a imagem
```
docker run "Nome da imagem  que foi feito o pull do docker hub
```

Comando para realizar o stop do container.<br/>
Obs: 1 - O comando abaixo mostra todos os comandos que executaram com sucesso
```
docker ps -a
```

2 - Após a execução do comando "docker ps -a", deverá aparecera lista abaixo com todos os container.

| CONTAINER ID | IMAGE |COMMAND|CREATED|STATUS|PORTS|NAMES|
|-------------|-------------|-------------|-------------|-------------|-------------|-------------|
| 1046b0c1ea85|hello-world  |"/hello"|2 minutes ago|Exited (0) 2 minutes ag|N/A| goofy_ |

3 - Para realizar o stop do container é necessário pegar o Id do container para realizar o stop do mesmo.
```
docker stop 1046b0c1ea85
```

Comando para remover o container do docker<br/>
Obs: Esse comando somente podera ser executado quando o container estiver parado.<br/>
```
docker rm 1046b0c1ea85
```