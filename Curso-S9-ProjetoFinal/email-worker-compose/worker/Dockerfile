FROM python:3.6
LABEL maintainer 'Aluno Cod3r <aluno at cod3r.com.br>'

# Variável de ambiente do Python settando o valor 1, para que desta forma ele possa executar os prints sem utilizar o buffer e executar de uma forma síncrona.
ENV PYTHONUNBUFFERED 1
# Instalar o redis fazendo papel que o arquivo app.sh estava fazendo.
RUN pip install redis==2.10.5

ENTRYPOINT ["/usr/local/bin/python"]