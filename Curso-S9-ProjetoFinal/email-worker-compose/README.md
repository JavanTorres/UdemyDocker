# Como rodar e testar apropriadamente

docker-compose up -d --scale worker=3

docker-compose logs -f -t

Chamar http://localhost:85/ e fazer grações, veja que worker_1, worker_2 e worker_3 irão trabalhar de forma intercalada.

Procure por "Mandando a mensagem:" no console e veja que são workers diferentes atuando sendo 3 no total.

Sai do console de logs, mas deixei o compose rodando os serviços e execute:

'docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails''

O comando acima vai entrar no container de BD e fazer um select para provar que os dados foram gravados.

docker-compose down