# Use uma imagem base do PostgreSQL
FROM postgres:latest

WORKDIR /app

# Variáveis de ambiente para personalizar a criação do banco de dados
ENV POSTGRES_USER=${POSTGRES_USER}
ENV POSTGRES_PASSWORD=${POSTGRES_PASSWORD}
ENV POSTGRES_DB=${POSTGRES_DB}
ENV POSTGRES_PORT=${POSTGRES_PORT}
ENV POSTGRES_HOST=${POSTGRES_HOST}


RUN apt-get update && apt-get -y dist-upgrade
RUN apt install -y netcat

COPY ./requirements.txt /app/requirements.txt

# Copie o arquivo SQL de inicialização para o diretório de inicialização do PostgreSQL
COPY . /app

RUN chmod +x /app/entrypoint.sh

CMD ["/app/entrypoint.sh"]
