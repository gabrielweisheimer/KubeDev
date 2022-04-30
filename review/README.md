## Passos para executar:

1) docker build -t gweisheimer/review-ms:0.1 -f Dockerfile ./src/Review.Web
2) docker push gweisheimer/review-ms:0.1
3) docker tag gweisheimer/review-ms:0.1 gweisheimer/review-ms:latest
4) docker push gweisheimer/review-ms:latest

# Serviço de Reviews

Esse projeto é um serviço de cadastro de reviews. Ele trabalha cadastrando o review de qualquer elemento.

## Estrutura do projeto

Esse projeto trabalha com uma base de dados Postgree 

![Diagrama](./img/diagrama.png)

## Configuração

É preciso determinar a connection string pra que ele acesse o banco de dados Postgree. Isso pode ser feito alterando o arquivo src/Review.Web/appsettings.json ou definindo como variável de ambiente (ConnectionStrings__MyConnection)

Exemplo:

ConnectionStrings__MyConnection: Host=localhost;Database=pguser;Username=pguser;Password=Pg@123;
