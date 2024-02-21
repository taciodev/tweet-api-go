# API de Tweets em Golang

Este é um desafio prático projetado para consolidar os conceitos aprendidos ao trabalhar com Golang. A aplicação consiste em uma API básica para criar, listar e deletar tweets.

## Funcionalidades

Desenvolvemos uma API de tweets que permite aos usuários realizar as seguintes operações:

- Listar todos os tweets
- Criar um novo tweet
- Deletar um tweet existente

## Como Usar

1. **Clonar o Repositório:**

```bash
git clone https://github.com/seuusuario/api-de-tweets.git
```

2. **Configurar o Ambiente:**

Certifique-se de ter o Go instalado em seu sistema. Se necessário, siga as instruções de instalação em [golang.org](https://golang.org).

3. **Executar o Servidor:**

```bash
go run main.go
```

4. **Interagir com a API:** Use um cliente HTTP, como curl ou Postman, para enviar requisições para os endpoints da API e realizar as operações desejadas.

## Endpoints da API

- **GET /tweets**: Retorna a lista de tweets.

Exemplo:

```bash
curl http://localhost:8080/tweets
```

- **POST /tweet**: Cria um novo tweet. Envie um JSON no corpo da requisição com o conteúdo do tweet.

Exemplo:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"content": "Este é um novo tweet!"}' http://localhost:8080/tweet
```

- **DELETE /tweet/{id}**: Deleta um tweet existente. Substitua {id} pelo ID do tweet que deseja deletar.

Exemplo:

```bash
curl -X DELETE http://localhost:8080/tweet/1
```

## Contribuindo

Contribuições são bem-vindas! Se você tiver sugestões de melhorias, abra uma issue para discutir suas ideias ou envie um pull request com suas alterações.

## Licença

Este projeto está licenciado sob a [MIT License](https://opensource.org/licenses/MIT). Sinta-se à vontade para usar, modificar e distribuir o código conforme necessário.
