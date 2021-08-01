### Ambiente de desenvolvimento Docker: PHP 7.4 | Mysql 8.0 | Nginx 1.21

## Pré-requisitos:
- Docker
- Docker-compose
- Git

# PHP - Versão 7.4
- Extensões: PDO_MYSQL
- Xdebug
- Composer

# Mysql - versão 8.0
- Porta: 3306
- Usuário: root
- Senha: root

# Nginx - versão 1.21
- http://localhost/
- Document root: /www/public

# Instalação
- git clone https://github.com/pedrohcmiguez/docker-dev.git
- cd docker-dev
- Iniciar: sudo docker-compose up -d

# Gerenciamento
- Atualizar a build do docker: sudo docker-compose up -d --build
- Parar: sudo docker-compose down -v
