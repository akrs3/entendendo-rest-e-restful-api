## Modelo de Maturidade Richardson - parte 1

* Leonard Richardson propôs um modelo de 4 nível para alcançar uma API REST

    - 0, 1 e 2 mais familiares, mais fáceis, mas não são consideradas REST

0. **POX:**

    - Mensagens podem ser serializadas JSON, XML ou outros
    EX:
        - Verbo HTTP: GET; 
        - URI: /buscarCLiente/1
        - Ação: Vizualizar

        - Verbo HTTP: POST
        - URI: /editarCLiente/1
        - Ação Editar

    - Uso dos verbos e nomes de recursos sendo usados de forma errada
    - Maniupulacao incorreta de códigos HTTP
    - **Nem mesmo usa o HTTP de forma certa**

