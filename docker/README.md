# Imersão Full Cycle 8 - Docker

Este projeto faz parte da **Imersão Full Cycle 8** e tem como objetivo ensinar conceitos e práticas relacionadas ao uso de **Docker** no desenvolvimento de aplicações modernas. Abaixo, você encontrará uma explicação detalhada sobre o projeto, como configurá-lo, executá-lo e entender os conceitos aplicados.

---

## Arquivo `test.http`

O arquivo `test.http` é utilizado para realizar testes de requisições HTTP diretamente, sem a necessidade de ferramentas externas como Postman ou cURL. Ele se enquadra na categoria de **testes de integração**, pois permite validar a comunicação entre a aplicação e outros serviços ou APIs, garantindo que os endpoints estejam funcionando conforme esperado.

### Como Utilizar o `test.http`

1. Certifique-se de ter uma extensão para manipular arquivos `.http` instalada no seu editor de código. Por exemplo:
    - [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) para Visual Studio Code.

2. Abra o arquivo `test.http` no editor.

3. Execute as requisições diretamente no editor, verificando as respostas retornadas pelos endpoints.

Este arquivo é especialmente útil para validar rapidamente os endpoints da aplicação durante o desenvolvimento, sem a necessidade de configurar ambientes externos.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

```
/home/etica/workspace/imersao-fullcycle-8/docker/
├── Dockerfile
├── docker-compose.yml
├── index.js
├── README.md
├── test.http
```

### Principais Arquivos e Diretórios

- **Dockerfile**: Define a imagem Docker para a aplicação.
- **docker-compose.yml**: Gerencia os serviços do projeto, como a aplicação e banco de dados.
- **src/**: Contém o código-fonte da aplicação.
    - **app/**: Diretório principal da aplicação.

---

## Pré-requisitos

Antes de começar, certifique-se de ter os seguintes itens instalados:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## Configuração do Ambiente

1. Clone este repositório:

     ```bash
     git clone https://github.com/seu-usuario/imersao-fullcycle-8.git
     cd imersao-fullcycle-8/docker
     ```

2. Construa a imagem Docker:

     ```bash
     docker build -t imersao-fullcycle-app .
     ```

3. Inicie os serviços com Docker Compose:

     ```bash
     docker-compose up -d
     ```

4. Acesse a aplicação no navegador em: [http://localhost:8080](http://localhost:8080)

---

## Conceitos Aplicados

- **Dockerfile**: Configuração da imagem Docker com base no Python.
- **Docker Compose**: Orquestração de múltiplos serviços.
- **Boas Práticas**: Estruturação de projetos e uso de ferramentas modernas.

---

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).