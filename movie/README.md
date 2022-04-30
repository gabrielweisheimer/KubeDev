## Passos para executar:

1) docker build -t gweisheimer/movie-ms:0.1 -f Dockerfile ./src
2) docker push gweisheimer/movie-ms:0.1
3) docker tag gweisheimer/movie-ms:0.1 gweisheimer/movie-ms:latest
4) docker push gweisheimer/movie-ms:latest


# Serviço de listagem de filmes

Esse projeto é um serviço de listagem de filmes. 

## Estrutura do projeto

Esse projeto trabalha com uma base de dados MongoDB e 

![Diagrama](./img/diagrama.png)

## Configuração

É preciso determinar a connection string pra que ele acesse o banco de dados MongoDB. Isso deve ser feito definindo a variável de ambiente MONGODB_URI

Exemplo:

MONGODB_URI: mongodb://mongouser:mongopwd@localhost:27017/admin