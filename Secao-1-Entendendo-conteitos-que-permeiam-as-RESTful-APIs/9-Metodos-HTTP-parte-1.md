## Métodos HTTP 

* Usados para criar uma API RESTful.

* Existem 9 tipos: 

1. GET

    - Usado quando é necessário obter recursos
    - Idempotente, independente do número de vezes que é executado sob um recurso, o resultado permanece
    - Não modifica dados
    - Ex: ```curl https://jsonplaceholder.typicode.com/posts/1 -i -v -X GET````
    - Mas nao é preciso o "-X GET" pois o GET já é o padrão do curl

2. POST

    - Usado para criar recurso
    - Ex de criação: 
    ``` curl -X POST https://jsonplaceholder.typicode.com/posts -H "Content-Type: application/json" -d '{"userId":1, "title": "Meu artigo", "body": "Corpo do artigo"}' ```

3. PUT

    - Atualizar um recurso
    - Só permite a subtituição inteira do recurso 
    - Ex:
     ``` curl -X PUT https://jsonplaceholder.typicode.com/posts -H "Content-Type: application/json" -d '{"userId":1, "title": "Meu artigo modificado", "body": "Corpo do artigo"}' ```

4. DELETE

    - Apagar um recurso
    - Ex: 
    ``` curl -X DELETE https://jsonplaceholder.typicode.com/posts/101 ```
