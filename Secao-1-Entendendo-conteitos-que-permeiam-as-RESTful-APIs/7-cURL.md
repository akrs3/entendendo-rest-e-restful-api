## cURL

* Documentação: [https://curl.haxx.se/]

* Ferramenta de linha de comando para pegar enviar arquivos através da sintaxe URL. Ela foi desenvolvida na linguagem C.

* Instalação:

    - Linux: ```supo apt-get install curl```
    - MAC: ```brew install curl```
    - Windows: ```https://www.cygwin.com```
    - Online: ```http://onlinecurl.com/```

* Requisição cURL é composta pela palavra curl, pela URL e um conjunto de opções que permite modificar coisa na requisição. As opções são:

    - **-H**: Atalho para HEADER. Substitui campos de cabecalho HTTP
        Ex: -H "Content-Type: application/json"

    - **-d**: Atalho para data, usado para envidar dados para JSON
        Ex: -d '{"name": "Anne Kelly"}'

    - **-i, include**: o cURL não mostrará só o corpo da resposta, mas também o cabeçalo/HEADER.

    -**-I, -head**: requisição do tipo HEAD, trazendo apenas o cabeçalho.

    - **-X, -request**: especifica qual verbo HTTP desejado. Padrão GET.

    - OBS: curl --help

* Testando: [https://jsonplaceholder.typicode.com/]
    ```curl -i https://jsonplaceholder.typicode.com/users/1```

