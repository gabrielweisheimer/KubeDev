## Passos para executar:

1) docker build -t gweisheimer/rotten-potatoes-ms:0.1 -f Dockerfile ./src
2) docker push gweisheimer/rotten-potatoes-ms:0.1
3) docker tag gweisheimer/rotten-potatoes-ms:0.1 gweisheimer/rotten-potatoes-ms:latest
4) docker push gweisheimer/rotten-potatoes-ms:latest

# Projeto Rotten Tomatoes Microsserviços

## Estrutura do projeto
Esse projeto é baseado em uma aquitetura de Microsserviços e depende de outros 2 projetos pra funcionar

- [Serviço de Filmes](https://github.com/kubedev/movie)
- [Serviço de Review](https://github.com/kubedev/review)

Segue abaixo o diagrama:

![Diagrama da solução](./img/diagrama.png)

## Configuração

MOVIE_SERVICE_URI => URL de acesso ao serviço de listagem de filmes

REVIEW_SERVICE_URI => URL de acesso ao serviço de listagem de reviews

Exemplo:

MOVIE_SERVICE_URI: http://movies:8181

REVIEW_SERVICE_URI: http://review:8282


