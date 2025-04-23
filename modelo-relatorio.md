# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 22/04/2025

Empresa: Abstergo Industries 

Responsável: Essias Alves Souza


## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries , realizado por Essias Alves Souza. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 

- AWS ECS - Elastic Container Service.
- Executar containers.
- A aplicação será distribuída, sendo servidor Web (Apache) e banco de dados (mySql). Para suportar a aplicação serão necessários dois containers, um para cada aplicação. Com o ECS será possível criar estes containers em
- poucos segundos.

Etapa 2: 
- AWS - EKS - Elastic Kubernetes Service.
- Orquestração de containers.
- O AWS EKS será necessário para orquestrar as execuções dos containers da seguinte maneira: caso haja uma quantidade elevada de execuções configuraremos o EKS para rodar novos containers e fazer o balanceamento de carga.

Etapa 3: 
- AWS S3 - Simple Storage Service.
- Armazenamento de objetos.
- Iremos armazenar os arquivos dos containers nos AWS S3 deixando dessa forma todos os arquivos salvos e acessíveis para qualquer container, inclusive arquivos de bancos de dados dos containers de banco de dados.  



## Conclusão
A implementação de ferramentas na empresa *Abstergo Industries  tem como esperado a redução de custos com infraestrutura de TI On-Premises*, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

[What is Amazon EKS?](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)

[What is Amazon Elastic Container Service?](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html)

[What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

Assinatura do Responsável pelo Projeto:

Essias Alves Souza
