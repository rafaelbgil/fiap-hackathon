## ADR 10. Uso de github actions para pipeline CI/CD

### Status
Aceito

### Contexto
Dado a necessidade de desenvolver o produto usando a metodogia ágil, fazendo com que hajam deploys mais frequentes e com menos alterações de artefatos por implementação.

### Decisão
Foi optado por desenvolver uma esteira de CI/CD e foi optado por utilizar o Github Actions. Entre os motivos de escolha do Github actions estão:
- Baixo custo de operação
- Facilidade para desenvolvemento de pipeline
- Integração nativa com ferramentas de terceiros.


### Consequências
Será necessário assegurar corretamente o permissionamento dos repositórios, afim de impedir que mudanças por pessoas não autorizadas sejam publicadas em produção.

### Conformidade
Após a implementação será possível verificar a execução dos jobs no github actions.