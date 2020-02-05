FROM postgres:11.6-alpine

ENV POSTGRES_DB=db \
    POSTGRES_USER=usr \
    POSTGRES_PASSWORD=pwd

# Put sql files in /docker-entrypoint-initdb.d
COPY datas/01-CreateScheme.sql /docker-entrypoint-initdb.d
COPY datas/02-InsertData.sql /docker-entrypoint-initdb.d
