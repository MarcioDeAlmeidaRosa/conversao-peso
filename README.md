# Conversão de peso
Api responsável por efetuar a conversão Grama para Quile e Quile para Grama.

## Build da imagem

Executar via prompt de comando dentro da pasta /src: </br></br>
`docker build -t marcioalmeidarosa/conversao-peso:1.0 .`</br></br>
O comando descrito acima irá gerar uma imagem local que você conseguirá ter acesso executando o comando: </br></br>
`docker images marcioalmeidarosa/conversao-peso:1.0`

## Executando o container com a imagem local

Executar via prompt de comando para executar o container com a imagem gerada: </br></br>
`docker run --name=api_conversao_peso_csharp -p 8020:80 -p 4443:443 -d marcioalmeidarosa/conversao-peso:1.0`</br></br>
Este comando irá listar os container em execução: </br></br>
`docker ps --filter name=api_conversao_peso_csharp`

## Enviando a imagem 1.0 local para o container register do docker

Executar via prompt de comando para enviar a imagem 1.0 gerada local para o container register docker hub: </br></br>
`docker push marcioalmeidarosa/conversao-peso:1.0`</br></br>

## Gerando image latest

Executar via prompt de comando para gerar image latest com base na image 1.0: </br></br>
`docker tag marcioalmeidarosa/conversao-peso:1.0 marcioalmeidarosa/conversao-peso:latest`</br></br>

## Enviando a imagem latest local para o container register do docker

Executar via prompt de comando para enviar a imagem latest gerada local para o container register docker hub: </br></br>
`docker push marcioalmeidarosa/conversao-peso:latest`</br></br>

## Visualizando a imagem enviada para o container register do docker
[Clique para acessar a imagem...](https://hub.docker.com/repository/docker/marcioalmeidarosa/conversao-peso)