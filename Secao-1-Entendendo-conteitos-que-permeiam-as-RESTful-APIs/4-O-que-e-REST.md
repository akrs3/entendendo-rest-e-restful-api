## REST

* Representational State Transfer (Transferência de Estado Representacional)

    - Formalizar conjunto de melhores práticas: "constraints"
    - Essas constraints tinham objetivo de determinar a forma na qual padrões como HTTP e URI deveriam ser modelados

* Constraints REST:

    - Cliente/Servidor:

        - É obrigatória
        - Separa responsabilidades das partes do sistema
        - Cliente: Front-end; Servidor: Back-end
        - Evolução e escalabilidade das partes diversas do sistema de forma independente

    - Stateless:

        - É obrigatória
        - Cada requisição deve ser independente, conter todas as ifnromações necessárias para ser tratada com sucesso pelo servidor. 
        - Não deve ter ligação com requisições passadas ou futuras.

    - Cache

        - É obrigatória
        - Para melhor performance, um sistema REST deve permitir que suas respostas sejam passíveis de CACHE
    
    - Interface Uniforme

        - É obrigatória
        - Bastante esforço deve ser feito para ter uma interface modelada e padronizada, considerando os elementos:
            - Recursos
            - Mensagens autodescritivas
            - Hypermedia
        - Interface que permita manilpulação de conceitos

    - Sistema em Camadas

        - É obrigatória
        - Capacidade de adicionar elementos intermediários que sejam transparentes  para seus clientes
        - Permitindo escalabilidade
        - Ex: Balanceador de Carga

    - Código Sob Demanda

        - É opcional
        - Aumenta a flexibilidade dos clientes
        - O código só é baixado quando for necessário
        - Essa prática reduz a visibilidade, pode gerar um problema de segurança
