Download da imagem do site do docker hub
```
docker pull yeasy/simple-web
```

Executar o site na porta 80
```
docker run --rm -it -p 8011:80 yeasy/simple-web:latest
```