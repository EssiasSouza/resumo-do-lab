# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA

Data: 25/04/2025

Empresa: Abstergo Industries 

Responsável: Essias Alves Souza

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Essias Alves Souza. O objetivo do projeto foi elencar 3 medidas de segurança em conjunto dos serviços da AWS, com a finalidade de realizar aumentar a segurança na empresa.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:

Medida 1: 
- Uso de IAM com Princípio do Menor Privilégio
Criaremos usuários e roles no IAM (Identity and Access Management) concedendo apenas as permissões estritamente necessárias para cada função.

Medida 2: 
- Ativação de MFA (Autenticação Multifator)
Habilitaremos o MFA para contas root e usuários IAM, adicionando uma camada extra de segurança além da senha.

Medida 3: 
- Criptografia de Dados
Usaremos criptografia para proteger dados em repouso (com KMS - Key Management Service) e em trânsito (com SSL/TLS).

## Conclusão
A implementação de ferramentas na empresa *Abstergo Industries tem como esperado o benefício de aumento de camadas de segurança para impedir perca da informação como também indisponibilidade e integridade*, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

[Perform a privileged task on an AWS Organizations member account](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user-privileged-task.html)

[Multi-factor authentication for AWS account root user](https://docs.aws.amazon.com/IAM/latest/UserGuide/enable-mfa-for-root.html)

[AWS Key Management Service Documentation](https://docs.aws.amazon.com/kms/)

Assinatura do Responsável pelo Projeto:

Essias Alves Souza
