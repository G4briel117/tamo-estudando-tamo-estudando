
Pensa nele como um **“estoque de peças”** que você pode usar em vários lugares da sua API, sem precisar repetir.

Dentro de `components` você pode guardar:

- **schemas** → modelos de dados (ex.: um objeto `Usuario` com `id` e `nome`).
    
- **responses** → respostas prontas (ex.: erro 404 ou sucesso 200).
    
- **parameters** → parâmetros usados em vários endpoints (ex.: `page`, `limit`).
    
- **requestBodies** → corpos de requisição comuns (ex.: envio de login).
    
- **securitySchemes** → definições de autenticação (ex.: Bearer Token, API Key).
    
- **headers, examples, links, callbacks** → outras coisas que também podem ser reaproveitadas.

```yaml
components:
  schemas:
    Usuario:
      type: object
      properties:
        id:
          type: integer
        nome:
          type: string

```

E depois, em qualquer lugar da sua API, você só **aponta para esse schema** com o `$ref`:

```yaml

responses:
  '200':
    description: Usuário retornado com sucesso
    content:
      application/json:
        schema:
          $ref: '#/components/schemas/Usuario'

```
