# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 03/09/2023
Empresa: Abstergo Industries 
Responsável: Arthur de Assis Ferrande

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Arthur de Assis Ferrande. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 
- Amazon EC2 (Elastic Compute Cloud)
- Provisionar instâncias para uso computacional, migrando o "on premises" para o cloud.
- Ao utilizar o EC2, podemos ter maior flexibilidade, escalabilidade e elasticidade do uso. Por ter seu pagamento como "pay as you go" no plano On Demand, conseguimos cortar custos já de início, já que pagamos somente pela capacidade computacional usada, e quanto mais usamos, menos pagamos. É possível diminuir mais ainda o custo ao utilizar os planos de 1 a 3 anos de contrato oferecidos pela AWS, como é o caso do Savings Plans ou Instâncias Reservadas. Podemos ainda atrelar um Auto Scaling Group, junto de um Load Balancer, facilitando a vida dos clientes e a disponibilidade do sistema. Entraremos em mais detalhes sobre o ASG na próxima etapa. Importante também provisionar em multi AZ, assim tendo proteção à falhas ou interrupções.

Etapa 2: 
- Auto Scaling
- Como o nome diz, escala automaticamente os recursos.
- O Auto Scaling ou Auto Scaling Group, de forma geral, auxilia na escalabilidade/elasticidade de certos itens provisionados na AWS. Como é o caso das instâncias EC2, dentre outros recursos. Com isso, e a devida configuração, deixamos de ter recursos ociosos, que ao não serem necessários serão interrompidos, mantendo apenas a quantia mínima que decidimos ou o suficiente para a manutenção das funcionalidades dada a carga de uso requerida em certo momento, consequentemente cortando gastos. O mesmo não é possível no on premise, a não ser que tiremos parte do nosso data center da tomada, o que geralmente não é possível ou recomendado. 
Caso a demanda seja alta, evitamos que nossos recursos "gargalem", pois serão provisionados automaticamente novos recursos, e podemos também decidir uma quantia máxima a ser provisionada. Assim auxiliando tanto na disponibilidade geral do nosso sistema sob uma carga mais alta que o normal, como no corte de custos, devido à elasticidade, quando essa carga for menor. Enquanto que, dada essa mesma situação no on premise, ao precisar escalar teríamos um custo fixo de antemão, além do tempo que levaria de transporte e montagem, sem a opção de diminuí-lo quando não estivesse sendo utilizado, além dos gastos com manutenção, energia, e afins.

Etapa 3: 
- Banco de Dados e Armazenamento
- Uso, gerenciamento e armazenamento de dados, com maior eficiência e segurança.
- Ao migrar nosso banco de dados e armazenamento para a AWS, temos algumas opções, as principais sendo: Amazon RDS ou Aurora para banco relacionais, o segundo com compatibilidade com MySQL e PostgreSQL, e o primeiro com mais opções, mas não somente nisso que se diferem. E DynamoDB, dentre outros para NoSQL. As vantagens de migrar o banco de dados para o Cloud é a diminuição de custos, além dos benefícios de velocidade, monitoramento, recuperação automática e autoescalabilidade. No caso do Aurora, por exemplo, o custo pode ser de um décimo do valor de um banco de dados comercial. Já no RDS, pode chegar a uma economia de 40% em média, em um período de três anos. Lembrando que se paga apenas pelo que usar, além das taxas por instância executada. Não sendo necessário se preocupar com manutenção e armazenamento, por não ter que provisionar excedente de antemão visando uso futuro. 
Se tratando de armazenamento, podemos realizá-los tanto no Elastic Block Store, como no S3, dependendo do caso e necessidade de uso. Pagando somente pelo o que provisionamos, em GB. Com snapshots ou versionamento para backup, durabilidade e disponibilidade altíssimas. Novamente, a diminuição de custos vem através da não necessidade de manutenção e gasto com hardware. 

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como objetivo diminuir gastos após realizar a migração de recursos do on premise para o cloud, aumentando eficiência e produtividade da empresa, e trocando gastos fixos, e de antemão - por vezes desnecessários - por cobranças flexíveis, junto a escalabilidade + elasticidade do negócio. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

https://aws.amazon.com/pt/ec2/  
https://aws.amazon.com/pt/ec2/pricing/  
https://docs.aws.amazon.com/pt_br/autoscaling/ec2/userguide/auto-scaling-groups.html  
https://docs.aws.amazon.com/pt_br/autoscaling/application/userguide/what-is-application-auto-scaling.html  
https://blog.awsfundamentals.com/unlocking-the-benefits-of-aws-rds-scaling  
https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/AuroraUserGuide/Aurora.Integrating.AutoScaling.html#Aurora.Integrating.AutoScaling.Add  
https://aws.amazon.com/pt/rds/  
https://aws.amazon.com/pt/rds/pricing/  
https://aws.amazon.com/pt/rds/aurora/  
https://aws.amazon.com/pt/rds/aurora/pricing/  
https://aws.amazon.com/pt/rds/aurora/features/#High_Performance_and_Scalability  
https://aws.amazon.com/pt/ebs/  
https://aws.amazon.com/pt/ebs/pricing/  
https://aws.amazon.com/pt/s3/  
https://aws.amazon.com/pt/s3/pricing/?nc=sn&loc=4  


Assinatura do Responsável pelo Projeto:

Arthur de Assis Ferrande
