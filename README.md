# TaskManager

Sistema de gerenciamento e agendamento de tarefas desenvolvido com Java, Spring Boot e arquitetura de microsserviços.

## Objetivo

O TaskManager foi desenvolvido para permitir o gerenciamento de tarefas, autenticação de usuários e envio de notificações automatizadas através de uma arquitetura desacoplada baseada em microsserviços.

## Arquitetura

O sistema é composto pelos seguintes serviços:

### Microsserviços

| Serviço | Responsabilidade |
|----------|----------------|
| Usuário | Cadastro e autenticação de usuários |
| Tarefas | Gerenciamento das tarefas |
| Notificação | Envio de notificações por e-mail |
| BFF | Centralização das chamadas dos serviços |

## Repositórios

- Usuário: https://github.com/LuccaLimaOliveira/usuario
- Agendador de Tarefas: https://github.com/LuccaLimaOliveira/agendador-tarefas
- Notificação: https://github.com/LuccaLimaOliveira/notificacao
- BFF: https://github.com/LuccaLimaOliveira/bff-agendadorTarefas

## Tecnologias

- Java 17
- Spring Boot
- Spring Security
- JWT
- PostgreSQL
- MongoDB
- Postman
- GitHub Actions
- Docker (em evolução)

## Fluxo da Aplicação

1. Usuário realiza login.
2. BFF recebe a requisição.
3. Serviço de usuário valida autenticação.
4. Serviço de tarefas registra, consulta tarefas e deleta se necessário.
5. Serviço de notificação envia lembretes programados.

## Próximas Evoluções

- Containerização com Docker
- Docker Compose
- Observabilidade
- Testes automatizados

## Autor

Lucca Lima de Oliveira
