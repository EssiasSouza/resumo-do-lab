# RESUMO do Lab Microsoft Azure - Localizando Serviços por Categoria

Eu aprendi que existem inúmeros serviços para suprir as diversas necessidades e todos estão organizados em categorias.
---
Em cada categoria também há uma divisão por assuntos como é o exemplo da Categoria `Análise`, há o assunto `Processamento de Big Data` com os itens:

 - Analysis Services
 - Custers HDInsight
 - Data Factories
 - Data Lake Analytics
 - Data Lake Storage Gen1
 - Azure databricks
 - Microsoft Graph data connect
 - O Azure HDInsight em clusters AKS
 
 Essa divisão permite com facilidade a localização do serviço dentro da console da Azure. 

---

## SLA E ALTA DISPONIBILIDADE

O  nível de acordo de serviço ou SLA (Service Level Agreement) é o tempo que o Cloud Provider oferece de disponibilidade do serviço. Quando o valor é 99% o tempo é de 1,68 hora por semana e 7,2 horas por mês. Se o SLA é de 99,9 o tempo já diminui significativamente para 10,1 minutos e 43,6 minutos por mês.

O criar uma máquina virtual é possível criar a máquina virtual com redundância em outros servidores ou localidade para aumentar a disponibilidade visando em algumas estratégias como é o caso de ambiente resistente no caso de uma catastrofe o ambiente pode estar disponível em outro lugar ou até mesmo aumentar a velocidade de acesso porque a informação será oriunda de vários lugares.

O que é importante alinhar bem na arquitetura do sistema é validar a infraestrutura que será usada até mesmo porque as cobranças pode aumentar demasiadamente. 

## Criação de máquina virtual / Imagem e Arquitetura

No painel de criação da máquina virtual é possivel ver o valor estimado que será cobrado pela máquina e sobre a responsabilidade.
É possível configurar itens como:
- Reinicio automática
- Monitoramento
- Discos
- Peças
- Modelo de redundância
