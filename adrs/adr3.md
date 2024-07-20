## ADR 3. Uso da aplicação rabbitmq para mensageria como um serviço do kubernetes

### Status
Aceito

### Contexto
Dado a decisão de utilizar mensageria, reportada no [ADR 2. Uso de mensageria](adr2.md), se faz necessário a escolha de uma aplicação a ser usada para prover essa finalidade.

### Decisão
Foi optado por utilizar a aplicação rabbitmq que será implementada como um serviço do kubernetes, motivos:

- Simplicidade, rapidez na implementação e economia de recursos financeiros, uma vez que utilizaremos uma infraestrutura já existente;
- Uso do protocolo amqp, permitindo no futuro substituição do rabbitmq caso necessário;
- Evitar "Lock-in" com soluções de cloud providers, uma vez que vários utilizam soluções próprias para mensageria e muitas não suportam o protocolo amqp.


### Consequências
Será necessário adicionar mais um componente ao kubernetes e realizar o monitoramento.

### Conformidade
Após a implementação será possível processar requisições de forma assíncrona, e no futuro caso seja necessário migrar de cloud provider o serviço de mensageria não precisará ser alterado.
