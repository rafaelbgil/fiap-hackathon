## ADR 7. Uso de Storage Object para arquivos anexos de prontuário

### Status
Aceito

### Contexto
Dado a necessidade de upload e compartilhamento de arquivos entre médico e paciente.

### Decisão
Foi optado por utilizar algum serviço de object storage, tais como: Amazon s3, google storage e azure blob storage.

Motivos para escolha:
- Baixo Custo;
- Serviço ofertado pelos principais provedores cloud;
- Disponibilidade alta (SLA geralmente superior a 99,99%);
- Apis e recursos para compartilhamento de arquivos de forma temporário.


### Consequências
Implementar a rotina de integração conforme a nuvem escolhida, em caso de mudança de cloud provider será necessário desenvolver uma nova rotina.

### Conformidade
Após implementação será possível identificar registros de buckets no provedor cloud.