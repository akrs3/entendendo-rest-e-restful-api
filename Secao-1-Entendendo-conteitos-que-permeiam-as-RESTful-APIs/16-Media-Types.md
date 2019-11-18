## Media Types

* String que define qual formato do dado 
* Divide-se em: **tipo/subtipo**

* o tipo pode ser: application, audio, example, image, message, video etc. Consulte [https://www.iana.org/assignments/media-types/media-types.xhtml]

* Exemplos:
    - application/json
    - application/xml
    - application/yaml

* O Media type é usado no Header. EX: "Accept: application/xml"
* Pode aceitar mais de um valor: EX: "Accept: aapplication/xml;q=0.5, application/xml;q=0.1"

* Perceba o uso do **quality factor (q)**, informa a ordem de preferência (entre 0 e 1)

* Media Type x Mime Type: a mesma coisa hahah [https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Basico_sobre_HTTP/MIME_types]

* Content-Type x Accept: 

    - Content-type: é o campo q identifica o conteudo da requisicao, em qur formato estou enviando ao servidor
    - Accept: o tipo que se espera receber do servidor