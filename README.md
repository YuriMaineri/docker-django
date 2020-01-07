# Criação do docker-compose para ambiente Django

# Como fazer a instação:
 - Criar um Dockerfile para rodar o pip com instalação dos pacotes do python e imagem
 - Criar 'requirements.txt' com o django>=2.0,<3.0 e psycopg2>=2.7,<3.0
 - Criar o docker-compose.yml definindo as imagens do pgsql e build do web

# Criação do projeto Django
 - docker-compose run web django-admin startproject NOME_APLICAÇÃO .

# Dar permissão ao usuário
 - sudo chown -R $USER:$USER .

# Conexão ao banco
 - vim NOME_APLICAÇÂO/settings.py

# Basta executar para rodar o docker
 - docker-compose up -d

 **parametro -d serve para rodar em backgroud**

 **use docker-compose down para parar o docker**

# Terá acesso ao site acessando:
 - localhost:8000
