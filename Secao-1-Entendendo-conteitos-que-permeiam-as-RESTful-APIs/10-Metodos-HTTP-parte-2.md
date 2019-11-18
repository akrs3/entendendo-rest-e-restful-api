## Métodos HTTP - PArte 2

* Métodos extras:

    5. HEAD

        - Retorna apenas o cabeçalho do recurso
        - Ex: 
        ``` curl -I https://jsonplaceholder.typicode.com/posts/1 ```

    6. PATCH

        - Altera parcialmente os recursos, modificando apenas valores específicos do recurso, ao invés de enviar todos os dados novamente. 
        - Ex:
        ``` curl -X PATCH https://jsonplaceholder.typicode.com/posts/3 -H "Content-Type: application/json" -d '{"title": "Meu novo titulo" }' ```

    7. OPTIONS

        - Usado para saber quais método são possíveis para cada recurso ou qual URL permitida
        - Access-Control-ALoow-Methods: contem os metodos possiveis
        - Links úteis: 
            - [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Methods]
            - [http://zacstewart.com/2012/04/14/http-options-method.html]
        - Ex: 
        ``` curl https://jsonplaceholder.typicode.com/posts -I -X OPTIONS ```

    8. TRACE

        - Ecoa de volta a requisicao recebida para o cliente saber se houve mudancas feitas pelo servidores intermediarios
