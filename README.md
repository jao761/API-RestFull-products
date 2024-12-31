
Fluxo da Aplicação
Inicialização:

O serviço product é configurado no Docker Compose e cria um container PostgreSQL com credenciais definidas.
O Spring Boot é iniciado, configurando-se para conectar ao banco PostgreSQL utilizando as credenciais definidas.
Fluxo de Requisições:

Cliente (Frontend ou Ferramenta como Postman):
Envia requisições HTTP (GET, POST, PUT, DELETE) para o servidor Spring Boot através de endpoints.
API Spring Boot:
Processa as requisições no controlador correspondente.
Utiliza repositórios JPA para acessar e manipular os dados no banco.
Retorna respostas HTTP ao cliente com os dados solicitados ou mensagens apropriadas.
Banco de Dados PostgreSQL:
Responde a consultas SQL feitas pela aplicação Spring Boot.
Persiste ou recupera dados dos produtos conforme solicitado.
Endpoints da API:

POST /products: Cria um novo produto.
GET /products: Retorna a lista de produtos.
GET /products/{id}: Retorna os detalhes de um produto específico.
PUT /products/{id}: Atualiza as informações de um produto.
DELETE /products/{id}: Exclui um produto.
