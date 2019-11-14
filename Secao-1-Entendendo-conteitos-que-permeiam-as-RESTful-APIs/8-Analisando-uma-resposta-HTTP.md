## Analisando uma resposta HTTP

* Testando requisição: [https://jsonplaceholder.typicode.com/]
    ```curl -i https://jsonplaceholder.typicode.com/posts/1```

* Resposta HTTP é dividida em 4 partes:
    
    - Start-Line (Linha de Incício - Obrigatória)
    - Header Fiels (Cabeçalho de Campos / POde ter 0 ou mais)
    - Empty Line (Linha em Branco - Obrigatória - separa o cabeçalho do corpo da mensagem)  
    - Message-Body (Corpo da mensagem - Opcional)

1. Start-Line

    - Request-Line: indica versao do HTTP usada. Ex: HTTP/1.1
    - Status-Line: representa o status da resposta. Ex: 200 OK

2. Header-Fields

    - Representa metadados da requisição e resposta HTTP. 

        - Content-Type: informa como a representacao será serializada/recebida
        - Content-Lenght: tamanho do corpo da mensagem em arquitectos
        - X-Powered-By: Header Fields não oficiais e por padrão começam com **X**.
            - Consulta em [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers]
            - Atualmente não deve se usar o **X** 

3. Empty Line

    - Delimita o fim do Header-Fields e inicio do Corpo da Mensagem

4. Message-body

    - Dados enviados como resposta do servidor

* Outra forma de fazer requisição: 
    ```curl -v -i https://jsonplaceholder.typicode.com/posts/1```