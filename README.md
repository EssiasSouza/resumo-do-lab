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

## Data Centers - Globo

O site datacenters.microsoft.com/globe/explore oferece um mapa interativo, em 2D ou 3D, que permite visualizar a localização dos datacenters da Microsoft ao redor do mundo. Ele exibe as regiões do Azure, suas geografias e outras informações relacionadas à infraestrutura global da Microsoft. O mapa pode ser filtrado por diferentes categorias e também oferece uma visão geral da presença global da plataforma Azure.

## Criação de Máquinas Virtuais e Área de Trabalho Remoto.

A criação de máquinas virtuais no Azure é bem simples e com diversas configurações que podem facilitar a gestão da infraestrutura. Todas as máquinas e recursos configurados no Azure precisam de um grupo de recursos e esta é segunda configuração ao criar uma máquina virtual. Além disso é possível configurar:

- Nome da máquina
- Região
- Zona de disponiblidade
- Tipo de segurança
- Sistema operacional
- Tamanhos
- Tipo de autenticação
- Criar um usuário administrador.
  
Entre outras configurações é possível também configurar:
- Disco
- Rede
- Gerenciamento
- Monitoração

E também é possível outras configurações muito úteis à ára de governança e configuração de máquinas virtuals como desktop remoto para facilitar a disponbilidade de máquinas para funcionários sem precisar de fornecer um computador ao usuário.

## Armazenamento

Parar fazer uma configuração de armazenamento a assinatura já vem configurada e deve ser escolhido o grupo de recursos. O nome da conta de armazenamento deve ter nome único.

OBS.: Conta de armazenamento é o nome do armazenamento que está sendo criado.

- Região - Deve ser escolhida de acordo com os requisitos de latência ou até mesmo custo.
- Desempenho - Pode ser escolhido o `Standard` ou `Premium` que irá determinar a latencia
- Redundância - Pode ser usada LRS (local), GRS (geográfica), ZRS (Zona) e GZRS(Zona geográfica) que determinará o tipo de redundância este armazendo deverá ter.

Outras configurações permitem a configuração do tipo de armazenamento se é e frio ou quente, configuração de rede, Criptografia e outras configurações.

### Menu: Armazenamento de dados

Configuração de armazenamento, recebimento, compartilhamento e organização de dados e arquivos do Azure.

- Containers - Gerenciamento de pastas (é possível também já configurar um backup)
- Compartilhamento de arquivos - Ferramenta para criar uma conexão usando o menu `Conectar` disponível para conexão SMB para Windows, Linux e Mac)
- Filas - Configuração de mensageria
- Tabelas - Criação de tabelas

### Migração de dados

É possível criar um projeto de migração que viabiliza migrar arquivos e dados da estrutura on-premisses para a cloud usando ferramentas como o AZ Copy ou ainda usando o Azure Databox

- AZ Copy é a aplicação mais simples e leve para usar no terminal para fazer o transportar arquivo e há disponibilidade para Linux, Windows e Mac.
- Azure Data Box - Modalidade de transporte de dados com um disco rígido que é enviado para cliente, o cliente escreve os dados no disco e encaminha de volta ao Azure para subir na Nuvem. O limite dessa modalidade é de 80TB
- Data Box Disk - Limite de 35TB
- Data Box Heavy - Limite de 800TB
- Data Box job - Limite de 1TB
Cada serviço do Azure Data Box possui valores diferentes.

### Gerenciador de Armazenamento do Microsoft Azure

Aplicação para gestão de armazenamento. Basta baixar, instalar e fazer a sincronização e a console irá mostrar as assinaturas, contas de armazenamento e mais.

## Identidade e segurança (ENTRA ID)

Todo usuário deve ser gerenciado no Azure através do Entra ID que determinará funções e permissões dos usuários. É diferente do RBAC pois os usuários gerenciados nessa seção terá permissão apenas para gerenciamento dentro do Entra ID com permissões para mudanças na gestão de usuários.

É possível criar usuários e convidar usuários externos, inclusive em grupo.

- Entra connect - Sincroniza os usuários do ambiente On-premisses para o ambiente de Cloud.

Uma conta deletada tem até 30 dias para ser recuperada.

### Defender for Cloud

Aplicação cloud native e hibrído que traz informações sobre a segurança do ambiente

- Recomendação de segurança - Validador de segurança e sugestão da segurança.

## CALCULADORAS DE CUSTOS

Existem duas calculadoras dentro do Azure. Um é ideal para as estimativas de preços dos recursos do Azure e a outra serve para cálculo de economia na migração de on-premises para o Azure.

Essa segunda calculadora é chamada de TCO (Total Cust Ownership), ou seja, é a calculadora de custo total de propriedade.

A importância do uso dessas calculadoras dá-se à necessidade de que a empresa precisa avaliar os valores e elencar o que faz sentido ou reduzir o risco de custos inesperados.

## Portal de confiança do serviço 

E um portal de governança com diversas ferramentas 

- Normas de auditoria que a Microsoft obedece para estar em compliance. É um local onde podemos validar quais são as regras de cada país e como são aplicadas.
- Bloqueio de recursos 
- Purview 