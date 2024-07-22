## ADR 9. Microserviços separados para medico e paciente

### Status
Aceito

### Contexto
Dado a necessidade de gerenciar perfils de usuários pacientes e médicos.

### Decisão
Foi optado por desenvolver um microserviço para médicos e outro para paciente.

Motivos:
- Maior facilidade para implementação de customização
- Possibilidade de implementar camadas adicionais de segurança somente no microserviço paciente e sua base de dados, tendo em vista que informações de saúde de usuários são informações sensíveis e de alto nível de criticidade para LGPD.


### Consequências
Está previsto duplicação de código.

### Conformidade
Após implementação será possível trabalhar de forma independente com os perfis de médicos e pacientes.