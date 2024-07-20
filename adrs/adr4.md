## ADR 4. Uso do Mongodb como serviço

### Status
Aceito

### Contexto
Dado a decisão de utilizar uma base de dados **nosql** para o microserviço **prontuário**.

### Decisão
Foi optado por utilizar a aplicação mongodb como serviço.

A decisão baseia-se no fato do mongodb ser uma solução conhecida e estável de mercado.

A opção de utilizar o mongodb como serviço se dá para diminuir a complexidade de sustentação do serviço do mongodb.


### Consequências
Será necessário investimento financeiro superior ao de se utilizar o mongodb implementado diretamente no kubernetes.

### Conformidade
Após a implementação será possível utilizar do banco dados nosql mongodb.
