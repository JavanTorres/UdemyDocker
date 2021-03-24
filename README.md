# UdemyDocker
Repositório criado para abrigar conhecimentos obtidos no curso "Docker: Ferramenta essencial para Desenvolvedores".

Repositório do Curso: https://github.com/cod3rcursos/curso-docker

É muito importante rodar rotineiramente 'docker volume prune' para liberar espaço em disco apagando volumes que não são mais utilizados.


Obter Shell no container Docker em execução:

docker exec -i -t 4d9de6c0fba1 /bin/bash

Acessar um Mongo:

docker container exec -it node-mongo-compose_db_1 mongo

Acessando os logs de um container, tipo um node rodando um app:

docker logs 243967adc88b