## ADR 11. Uso do sonarcloud para análise de qualidade e segurança de código

### Status
Aceito

### Contexto
Dado a necessidade de assegurar a qualidade de código, cobertura de testes e segurança.

### Decisão
Foi optado por utilizar a ferramentar sonarcloud, a qual é um serviço em nuvem do sonarqube. Entre os principais motivos da escolha estão, custo baixo para implementação e experiência do time com o uso da ferramenta.


### Consequências
Será necessário ajustar as pipelines de CI/CD com um novo passo de análise de código usando o sonarcloud.

### Conformidade
Após a implementação será possível verificar as recomendações e status geral do código por meio da plataforma sonarcloud.