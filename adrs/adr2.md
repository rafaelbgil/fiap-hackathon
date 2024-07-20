## ADR 2. Uso de mensageria

### Status
Aceito

### Contexto
Dado a necessidade de assegurar que a solução desenvolvida tenha alta capacidade de escalabilidade e disponibilidade.

### Decisão
Foi optado por utilizar serviços de mensagem para comunicação assíncrona entre serviços que não necessitem de retorno imediato para o paciente.

Exemplo de serviços assíncronos: Cobrança e Notificação


### Consequências
Será necessário adicionar mais um componente a arquitetura e realizar o monitoramento adequado, de forma a garantir que mensagens não fiquem por tempo indeterminado na fila.

### Conformidade
Após a implementação será possível processar requisições de forma assíncrona, evitando assim sobrecarga do sistema.
