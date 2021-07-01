#Repositório para acompanhar curso Alura - Modelagem de banco de dados: Começando com NoSQL

```
Instalação de Docker com MySQL para executar comandos
$ docker run --name alura -p 3306:3306 -e MYSQL_ROOT_PASSWORD=qwe123 -d mysql:8

# Conectar no banco e executar SQL (sqls/ExportEmpresa.sql) para criar estrutura.

# Aula 2: Como exibir,consultar, filtrar e agrupar dados usando campos do tipo JSON no MySQL. (sqls/aula2)

Instalação de Docker com MongoDB para executar comandos
$ docker run --name alura-mongodb -p 27017:27017 -d mongo:4.4

```

```
# no Docker conectar no CLI do container e executar os comandos abaixo para
# criar database "empresa" e coleção "funcionario":

$ mongo
$ use empresa
$ db.funcionario.insertOne({x:1}) 
```

```
$ mongo

# exibir dados
$ db.funcionario.find()

# incluir mais de um documento
$ db.funcionario.insertMany([{..}, {..}, {..}]) 
```