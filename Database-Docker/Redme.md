Fonte:
```
https://johnfercher.medium.com/mysql-docker-7ff6d50d6cf1

```

1 - Docker build -> Constrói a imagem de acordo com o arquivo DockerFile.
Obs: O comando abaixo deverá ser executado dentro da pasta raiz onde esta o arquivo dockerfile.
Docker desktop, deverá estar aberto para execução do comando abaixo.

```
docker build -t backoffice-db .
```

2 - Executar o container com as devidas variáveis de ambiente

```
docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=RootPassword -e MYSQL_DATABASE=Backoffice -e MYSQL_USER=MainUser -e MYSQL_PASSWORD=MainPassword backoffice-db
```

3 - Para pegar o container_id execute o comando abaixo
Obs: O mesmo retorna um <b>id do container</b> para ser utilizado no passo 4. 
```
docker ps
```

4 - Acesso Manual ao Banco
Para obter o container_id basta executar o comando docker ps.
```
docker exec -it container_id bash
root@35e303abc71d23baea51d992f9d251c3db5f68e7fb2aa2570c980f44602b22a4:/# mysql -uroot -p
Enter password: RootPassword
```








