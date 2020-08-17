# API-REST-RESTFUL

Clente(client)


Acronimo de Aplication Programming Interface ( Interface de Programação de Aplicações ) é basicamente um conjunto de rotinas e padrões estabelecidos por uma aplicação, para que aoutras aplicações possam utilizar as funcionalidade desta aplicação.

- Responsável por estabelecer comunicação entre deferentes serviços.

- Meio de campo entre as tecnologias.

- Intermediador para troca de informações.

## REST


Um acrônimo para Representational State Transfer (
    Tranferência d de EStado Represebtativo).
)

Será feito a tranferência de dados de uma maneira simbólica,
 figurativa, representativa, de maneira didática.

 A tranferência de dados, geralmente, usando um protocolo HTTP.

 o Rest, delimita algums obrigações nessas tranferências de dados.

 Resources seria então, uma entidade, um objeto.
 
 ### 6 NECESSIDADES ( constraints ) para ser RESTful

 -_Client-Server_: Separação do cliente e do armazenamento 
 de dados (Servidor), dessa forma, poderemos
 ter uma portabilidade do nosso sistema, usando o o React para WEB e
 React Native para Smartphone, por Exemplo.

 -_Stateless_: Cada requisição que o cliente faz para o 
 servidor, deverá conter todas as informações necessárias
para o servidor entender e responder ( RESPONSE )  a requisição
(REQUEST). Exemplo: A sessão do usuário deverá ser enviada
em todas as requisições, para saber se aquele usuário está
autenticado e apto a usar os serviços, e o servidor não pode
lembrar que o cliente foi autenticado na requisição
anterior. Poderemos usar tokens para as comunicações.

-_Cacheable_: As respostas para uma requisição, deverão ser
explicitas ao dizer se aquela requisição, pode não ser
cacheada pelo cliente.

-_Layered System_: O cliente acessa a um endpoint, sem
precisar saber da complexidade, de quais passos estão sendo
necessário para o servidor responder a requisição, ou 
quais outras camadas o servidor está lidando, para que a
 requisição seja respondida.

 -_Code on demand (optional)_: Dá a possibilidade da nossa
 aplicação pegar códigos, como o JavaScript, por exemplo, e
 execultar no cliente.
 
  ## RESTFUL

 - RESTful, é a aplicação dos padrões REST.

 ## BOAS PRÁTICAS

 - Utilizar verbos HTTP para nossas requisições.
 - utilizar plural ou singular na criação dos endpoint? _NÃO IMPORTA_ use um padrão !
 - Não deixar barra no final do endpoint.
 - Nunca deixe o cliente sem resposta!

### VERBOS HTTP

 - GET: Receber dados de um Resource.
 - POST: Enviar dados ou informações para serem processadas por um Resource.
 - PUT: Atualizar dados de um Resouce.
 - DELETE: Deletar um Resouce.

 ### STATUS DAS RESPOSTAS
- 1xx: Infomação
- 2xx: Sucesso
   - 200: OK
   - 201: CREATED
   - 204: Não tem conteúdo PUT POST DELETE
- 3xx: Redirection
- 4xx: Client Error
   - 400: Bad Request
   - 404: Not found
- 5xx: Server Error
   - 500: Internal Server Error 
