<h3 style="font-size: 24px;"># Site do docker</h3>
https://www.docker.com/

<h3 style="font-size: 24px;"># Site do hub docker</h3>
https://hub.docker.com/

<h3 style="font-size: 24px;"># Comandos docker </h3>
https://stack.desenvolvedor.expert/appendix/docker/comandos.html

<h3 style="font-size: 24px;"># Verificar a versão do docker</h3>
 docker version

<h3 style="font-size: 24px;"># Comando para realizar o download da imagem para máquina local.</h3>
docker pull imagem "Nome da imagem do docker hub"

<h3 style="font-size: 24px;"># Comano para listar todas as imagens do docker.</h3>
docker imagem ls

<h3 style="font-size: 24px;"># Comando para listar os container.</h3>
docker ps    -> Somente é necessario verificar os container em execução.
docker ps -a -> Exibe os container que executaram e finalizaram por algum motivo.

<h3 style="font-size: 24px;"># Comando para iniciar a imagem</h3>
docker run "Nome da imagem  que foi feito o pull do docker hub

<h3 style="font-size: 24px;"># Comando para parar o container</h3>
1 - O comando abaixo mostra todos os comandos que executaram com sucesso
docker ps -a

2 - Após a execução do comando "docker ps -a", deverá aparecera lista abaixo com todos os container.

| CONTAINER ID | IMAGE |COMMAND|CREATED|STATUS|PORTS|NAMES|
|-------------|-------------|-------------|-------------|-------------|-------------|-------------|
| 1046b0c1ea85|hello-world  |"/hello"|2 minutes ago|Exited (0) 2 minutes ag|N/A| goofy_ |

3 - Para realizar o stop do container é necessário pegar o Id do container para realizar o stop do mesmo.
docker stop  1046b0c1ea85

<h3 style="font-size: 24px;"># Comando para remover o container do docker</h3>
Obs: Esse comando somente podera ser eecutado quando o container estiver parado.<br/>
docker rm 1046b0c1ea85

















