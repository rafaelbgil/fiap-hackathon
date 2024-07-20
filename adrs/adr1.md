## ADR 1. Uso de arquitetura de microserviços e Kubernetes 

### Status
Aceito

### Contexto
Dado a necessidade de assegurar que a solução desenvolvida tenha alta capacidade de escalabilidade e disponibilidade.

### Decisão
Foi optado por desenvolver uma arquitetura baseada em microserviços com Kubernetes.

A arquitetura baseada em microserviços facilita a escalabilidade de serviços especificos, não sendo necessário escalar toda a aplicação.

O Kubernetes é uma ferramenta consolidada no mercado para orquestração de containers, sendo suportado pelas principais plataformas cloud do mercado.

### Consequências
Será necessário investimento de tempo e dinheiro em soluções complementares para observabilidade da arquitetura, ex: monitoramento, logs centralizados, entre outros.

### Conformidade
Após a implementação será possível escalar os microserviços de forma individual baseada na carga e uso individuais de cada um, fazendo com que tenhamos uma rápida resposta para escalar.
