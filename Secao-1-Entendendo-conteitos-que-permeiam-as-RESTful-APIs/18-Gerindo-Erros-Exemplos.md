## Gerindo Erros (Exemplos)

- Ex1: API com apenas metodo GET

    - curl -i -X PUT http://example.com/users
    - HTTP/1.1 404 Not Found 
    - Podia ser usado o 405 method Not Allowed

- Ex2: cliente solicita representacao XML que nao está no servidor

    - o codigo retornado devia ser 406 Not Acceptable
    - curl -i http://example.com/users -H "Accept: xyz/abc"

