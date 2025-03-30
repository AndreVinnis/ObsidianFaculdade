# Métodos HTTP
Um método HTTP define a ação que um cliente deseja realizar quando faz uma requisição para um servidor web. Esses métodos são usados em APIs RESTful e em qualquer comunicação baseada em HTTP. 
Uma chamada HTTP é constituída por pelo verbo e seu endpoint. Costuma ter uma resposta no padrão JSON.

CRUD (**Create, Read, Update, Delete**) são as operações básicas de manipulação de dados e, no REST, são mapeadas para métodos HTTP.

Como funciona uma requisição HTTP?
Uma requisição HTTP funciona por meio de uma URI (é um identificador único que aponta para um recurso na web, podendo ser um site, uma API, um documento ou qualquer outro recurso acessível via rede.) 

http://api.exemplo.com:443/users/1
http:// - Esquema (protocolo)
localhost: - Host (domínio do servidor)
8080 - Porta 
/user/1 - Caminho (Endpoint)
## VERBOS HTTP
- GET: Receber dados de um Resource.
- POST: Enviar dados ou informações para serem processados por um Resource.
- PUT e PATCH: Atualizar dados de um Resource.
- DELETE: Deletar um Resource

## STATUS DAS RESPOSTAS
- 1xx: Informacional (Requisição em andamento)
- 2xx: Sucesso (Tudo ocorreu como esperado)
    - 200: OK
    - 201: CREATED
    - 204: Não tem corpo da requisição PUT POST DELETE
- 300: Redirecionamento (O cliente precisa tomar outra ação)
- 4xx: Client Error (O cliente precisa tomar outra ação)
    - 400: Bad Request
    - 404: Not Found!
- 5xx: Server Error 500: Internal Server Error
	- 500: Erro genérico do servidor
	- 504: O servidor demorou muito para responder