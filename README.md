# ia-classificacao

## Descrição

O projeto `ia-classificacao` é uma aplicação que utiliza o n8n e PostgreSQL para realizar classificações de dados de forma eficiente e automatizada. Este repositório contém as configurações necessárias para rodar o n8n e PostgreSQL utilizando Docker.

## Pré-requisitos

- [Docker](https://www.docker.com/get-started) instalado em sua máquina.
- [Docker Compose](https://docs.docker.com/compose/install/) instalado.

## Instalação

1. **Clone o repositório**

   ```bash
   git clone https://github.com/WenerSantos3/ia-classificacao.git
   cd ia-classificacao
   ```

2. **Configuração do ambiente**

   Ajuste as variáveis de ambiente no arquivo `docker-compose.dev.yml` conforme suas necessidades.

3. **Inicie os serviços**

   Execute o comando abaixo para iniciar o n8n e PostgreSQL em contêineres Docker:

   ```bash
   docker compose -f "docker-compose.dev.yml" up -d --build
   ```

## Uso

Após iniciar os serviços, você pode acessar o n8n pelo navegador em `http://localhost:5699`. Use as credenciais de autenticação definidas nas variáveis de ambiente para acessar a interface.

## Tecnologias

Tecnologias utilizadas no projeto

| Tecnologia                                | Descrição                                                                                            |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| [n8n](https://n8n.io/)                    | Plataforma de automação de workflows que permite integrar diversas aplicações e serviços.            |
| [PostgreSQL](https://www.postgresql.org/) | Sistema de gerenciamento de banco de dados relacional, conhecido por sua robustez e flexibilidade.   |