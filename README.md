# Projeto Sprint 04 - OdontoPrev
## Descrição do Projeto
Este projeto é uma aplicação Java desenvolvida para o gerenciamento de informações odontológicas, incluindo cadastros de pacientes, tratamentos e integração com mensageria RabbitMQ para comunicação assíncrona entre serviços. A aplicação utiliza Spring Boot como framework principal e contempla funcionalidades REST para CRUD (Create, Read, Update, Delete) das entidades do sistema.
O foco principal é permitir a manipulação e consulta dos dados odontológicos de forma eficiente, garantindo comunicação desacoplada via RabbitMQ para processos assíncronos, além de contar com internacionalização e outras funcionalidades.
---
## Pré-requisitos
Antes de rodar o projeto, certifique-se de que você tem instalado e configurado os seguintes itens:
- **Java JDK 17+** (compatível com o projeto)
- **Maven 3.6+** para build e gerenciamento de dependências
- **RabbitMQ** (servidor de mensageria) instalado e rodando localmente
- **MongoDB** (caso o projeto utilize banco NoSQL, verificar no código)
- **IDE** de sua preferência (IntelliJ IDEA, Eclipse, VSCode, etc.)
---
## Como rodar o projeto localmente
1. Clone este repositório ou extraia o ZIP do projeto.
2. Certifique-se de que o RabbitMQ está instalado e em execução localmente.
  - Para iniciar o RabbitMQ manualmente:
    - Windows: usar o serviço RabbitMQ instalado ou rodar via linha de comando se configurado.
    - Linux/Mac: rodar `rabbitmq-server` no terminal.
  - O RabbitMQ padrão roda na porta 5672.
3. Configure as variáveis de ambiente ou arquivo `application.properties` / `application.yml` com as credenciais do RabbitMQ, MongoDB e outras configurações necessárias.
4. No terminal, dentro da pasta do projeto, execute o comando Maven para buildar e rodar a aplicação:
  ```bash
  mvn clean spring-boot:run
