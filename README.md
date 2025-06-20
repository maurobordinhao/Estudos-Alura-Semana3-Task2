# Estudos-Alura-Semana3-Task2

Baseado no curso e mentoria Alura: Docker criando e gerenciando containers

1 - Criando uma rede bridge Docker:

$ docker network create --driver bridge minha-rede

2 - Subir um container do MongoDB:

$ docker run -d --network minha-rede --name meu-mongo mongo:4.4.6. 

3 - Suba a aplicação:

$ docker run -d --network minha-rede --name alurabooks -p 3000:3000 aluradocker/alura-books:1.0. 

O acesso na aplicação, deve ocorrer pela url localhost:3000, para carregar os dados do banco: localhost:3000/seed, e por último recarregar localhost:3000 para que as informações sejam exibidas.
