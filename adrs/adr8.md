## ADR 8. Uso de Mysql como serviço DBAAS

### Status
Aceito

### Contexto
Dado a necessidade de utilização de bases de dados SQL para os microserviços.

### Decisão
Foi optado por utilizar serviços DBAAS com o banco de dados mysql.

Motivos:
- Facilidade para implementação;
- Backup integrado;
- Restauração de backup fácil via interface;
- Criação de réplica de forma simples via interface;


### Consequências
Investimento maior em cloud se comparado ao de contratar uma máquina virtual e gerenciar o banco mysql de forma independente.

### Conformidade
Após implementação será possível identificar a instancia e base dados diretamente na interface web do provedor cloud.