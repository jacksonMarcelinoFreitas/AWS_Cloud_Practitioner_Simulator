# Simulado AWS Cloud Practitioner 2/5 

## Pergunta 1: 
Qual é o serviço de mensagens desenvolvido para Apache Active MQ e Rabbit MQ que
torna as integrações com sistemas legados desacoplados mais fáceis e que permitem o
uso de arquiteturas híbridas?

- [ ] sas
- [ ] SNS
- [X] Amazon MQ
- [ ] Kafka

### Explicação

**Correta**

Amazon MQ foi especificamente desenvolvido para atender essas stacks de tecnologia
https://aws.amazon.com/amazon-mq/?c=ai&sec=srv&amazon-mq.sort-
by=item.additionalFields.postDateTime&amazon-mq.sort-order=desc

**Incorretas**

O SNS - Simple Notification Service é utilizado para a troca de mensagens através do
esquema de Pub/Sub e tópicos, na AWS.<br>
O SQS - Simple Queue Message é um serviço de mensageria para troca de mensagens e
desacoplamento para arquiteturas AWS.<br>
O Kafka é um serviço utilizado para arquiteturas orientadas a eventos, mas não é um
serviço da AWS, apesar de ser possível sua utilização na plataforma.

#

## Pergunta 2:

Você está criando uma rede virtual isolada para os seus recursos dentro da AWS e deseja
separar a camada de servidores de dados da camada de servidores de aplicação. A
solução é criar duas sub-redes (subnets), uma para dados e uma para a aplicação. Qual é
o serviço que permite esse tipo de organização?

- [X] VPC
- [ ] ELB
- [ ] AWS Budget
- [ ] AWS Organizations

### Explicação

**Correta**

A VPC é uma rede privada virtual que é criada junto com a conta e que permite a criação
de subredes dentro dela para fazer esse tipo de separação para hospedar os recursos
computacionais.<br>
Além da VCP que é criada com a conta, também é possível criar outras, de acordo com a
necessidade do cliente.<br>
https://aws.amazon.com/vpc/?nc2=h_ql_prod_fs_vpc&vpc-blogs.sort-
by=item.additionalFields.createdDate&vpc-blogs.sort-order=desc

**Incorretas**

AWS Organizations é o serviço que permite organizar diversas contas da AWS para
unificá-las para diversas finalidades, como conSQLidação de custos por exemplo.
AWS Budget é o serviço que te permite estipular um valor de orçamento para monitorar e
enviar uma mensagem se o mesmo for excedido ou se aproximar de um % configurado.<br>
AWS ELB é o serviço para distribuir o tráfego de dados entre instâncias EC2


#

## Pergunta 3: 

O que pode ser feito como a AWS CLI (Command Line Interface) após baixá-la e
configurá-la no seu computador? (Selecione 2 alternativas)

- [ ] Realizar o login utilizando o MFA
- [X] Automatizar serviços da AWS
- [X] Controlar múltiplos serviços da AWS
- [ ] Visualizar gráfico de Custo de serviços da AWS

### Explicação

**Correta**

A Interface da Linha de Comando (CLI) da AWS é uma ferramenta unificada para o
gerenciamento de seus serviços da AWS. Com apenas uma ferramenta para fazer
download e configurar, você poderá controlar vários serviços da AWS pela linha de
comando e automatizá-los usando scripts
https://aws.amazon.com/cli/?nc2=h_ql_prod_dt_cli

**Incorretas**

As outras opções só podem ser feitas através do ConSQLe Web com Interface Visual pelo
Browser.

#

## Pergunta 4: 

Seu time de desenvolvimento está planejando modernizar um sistema e redesenhá-lo
dentro da AWS. Um dos requisitos não funcionais é a redução de interdependência para
minimizar falhas que acontecem e impactam outros componentes. Qual dos seguintes
conceitos se refere a esse requisito?

- [X] Desacoplamento
- [ ] Segregação
- [ ] Agregação
- [ ] Integração

### Explicação

**Correta**

Desacoplamento é um conceito de arquitetura de sistemas distribuídos, que permite que
os sistemas sejam desenvolvidos de forma independente e que suas integrações sejam
realizadas através de um serviço de mensageria como o SQS, SNS, etc. Uma das
vantagens deste tipo de implementação é evitar que falhas em alguns serviços e
sistemas não parem o processo como um todo até que os problemas estejam reSQLvidos.
https://docs.aws.amazon.com/prescriptive-guidance/latest/modernization-mainframe-
decoupling-patterns/queue.html

**Incorretas**

Integração é um conceito que está num nível de abstração maior, podemos ser
integrações acopladas ou desacopladas Agregação e Segregação são conceitos de
outras disciplinas de sistemas.

#

## Pergunta 5: 

Com a AWS você pode obter descontos baseados em volume e obter economias
substanciais à medida que o seu uso aumenta. Em qual serviço abaixo a definição de
preço é feita em camadas e quanto mais você usar, menor será o preço por GB?

- [ ] Lambda
- [X] S3
- [ ] EKS
- [ ] ECS

### Explicação

**Correta**

https://aws.amazon.com/pt/pricing/?nc2=h_ql_pr_ln

**Incorretas**

Os demais serviços são cobrados pelo uso de computação sob demanda

#

## Pergunta 6: 

Qual serviço da AWS que, além de ajudar na visualização dos cinco serviços que mais
aumentam os custos de uma conta, disponibiliza um detalhamento minucioso sobre
todos os recursos utilizados?

- [ ] AWS Billing
- [ ] AWS Budget
- [X] AWS Cost Explorer
- [ ] AWS Pricing

### Explicação
**Correta**

AWS Cost Explorer - https://aws.amazon.com/pt/aws-cost-management/aws-cost-explorer/?nc2=h_ql_prod_cm_cex

**Incorretas**

O AWS Budget é utilizado para criar orçamentos e alertas para gerenciar o uso dos
serviços da AWS.<br>
AWS Billing e Pricing não são serviços existente.

#

## Pergunta 7: 

Sua equipe de desenvolvimento está montando uma pipeline de CI/CD para uma nova
aplicação na AWS, qual serviço eles precisam incluir no final da esteira para implantar a
aplicação nos servidores de forma automatizada?

- [ ] AWS CodeCommit
- [ ] AWS Git
- [ ] AWS Deploy
- [X] AWS CodeDeploy


### Explicação

**Correta**

O AWS CodeDeploy é um serviço totalmente gerenciado de implantação que automatiza
implantações de software em diversos serviços de computação como Amazon EC2, AWS
Fargate, AWS Lambda e servidores locais. O AWS CodeDeploy facilita o lançamento
rápido de novos recursos, ajuda a evitar tempo de inatividade durante a implantação de
aplicativos e lida com a complexidade de atualizá-los. Você pode usar o AWS
CodeDeploy para automatizar implantações de software e eliminar a necessidade de
operações manuais propensas a erros. O serviço é dimensionado para estar de acordo
com as suas necessidades de implantação - 
https://aws.amazon.com/pt/codedeploy/

**Incorretas**

AWS CodeCommit é semelhante ao GitHub, GitLab, é uma solução da AWS para fazer versionamento e gestão de código fonte.<br>
AWS Deploy não existe, todos os serviços de CI/CD para desenvolvedores tem o Code" no. nome. CodePipeline, CodeCommit, CodeBuild, CodeArtifact, CodeDeploy<br>
AWS Git não existe. Git é a tecnologia utilizada para trabalhar com o codeCommit

#

## Pergunta 8: 

Sua empresa possui diversas áreas que devem construir suas aplicações dentro da AWS
usando templates de infraestrutura pré-definidos pelo time de arquitetos. As SQLuções
deverão ser implementadas como código IAC (Infra as Code). Qual serviço pode ser
utilizado para essa finalidade?

- [ ] Cloud Stacks
- [X] AWS CloudFormation
- [ ] AWS Config
- [ ] Cloud Templates

### Explicação

**Correta**

O AWS CloudFormation permite modelar, provisionar e gerenciar recursos da AWS e de
terceiros ao tratar a infraestrutura como código. Como código, a infraestrutura pode ser
alterada, versionada e automatizada para atender diversos requisitos de uma
implementação de infraestrutura, como o apresentado na questão. Template (modelo) é
o nome dado ao arquivo onde são declarados todos os serviços necessários na
infraestrutura desejada.<br>
https://aws.amazon.com/pt/cloudformation/

**Incorretas**

AWS Cloud Template e AWS Stacks não existem.<br>
Template é o arquivo onde você codifica a sua infraestrutura<br>
Stack é o conjunto de serviços criados com um template<br>
AWS Config é um serviço utilizado para gerenciar configurações padrão de diversos
serviços.

#

## Pergunta 9: 

Você está implementando um microsserviço para realizar análise de crédito SQLicitada
pelos seus clientes. A resposta desta análise deverá ser enviada para um sistema de
vendas, um sistema de empréstimos, e também para, um serviço de log do próprio
microsserviço. Qual serviço daAWS é o mais indicado para implementar essas e futuras
integrações de uma forma rápida?

- [ ] AWS Docker
- [ ] AWS Lambda
- [X] AWS SNS
- [ ] AWS ECS

### Explicação

**Correta**

Um dos possiveis usos do SNS é a integração de sistemas através da função Pub/Sub
que traz diversas possibilidades para o desenvolvimento das aplicações como realizar
essas integrações<br>
https://aws.amazon.com/sns/?c=ai&sec=srv&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc

**Incorretas**

AWS Docker não existe, entretanto o ECS - Elastic Container Service é o serviço
utilizado para implementar container na AWS, mas que não tem a finalidade do serviço
abordado na ## Pergunta.<br>
O AWS Lambda é utilizado para implementar funções sem servidores em diversas
linguagens de programação disponíveis.

#

## Pergunta 10: 

Se você quer desenvolver uma aplicação em Java ou qual das seguintes ferramentas
você pode usar?

- [ ] AWS ConSQLe
- [ ] AWS CLI
- [X] AWS SDK
- [ ] AWS IDE

### Explicação

**Correta**

AWS SDK
https://aws.amazon.com/tools/

**Incorretas**

AWS CLI - é a Interface da Linha de Comando (ILC) da AWS, que é uma ferramenta
unificada para o gerenciamento de seus serviços da AWS. Com apenas uma ferramenta
para fazer download e configurar, você poderá controlar vários serviços da AWS pela
linha de comando e automatizá-los usando scripts<br>
AWS ConSQLe é a interface web onde você pode gerenciar sua conta e seus serviços<br>
AWS IDE não é um serviço que não existe na AWS.

#

## Pergunta 11: 

Selecione as opções verdadeiras que ser referem ao AWS IAM? (selecione 3 alternativas)

- [X] Permissões determinam se a requisição é permitida ou negada
- [X] A maioria das Policies são armazenadas em documentos JSON
- [ ] Policy é um documento que todos os usuários devem assinar digitalmente quando acessam a AWS pela primeira vez
- [X] Policy é um objeto da AWS que quando associado a um usuário ou recurso define suas permissões

### Explicação

Os 3 itens estão relacionados a Policies do AWS IAM<br>
https:Wdocs.aws.amazon.com/lAM/latest/UserGuide/introduction_access-
management.html

#

## Pergunta 12: 

Qual é o serviço da AWS utilizado para migrar banco de dados de forma rápida e segura?

- [ ] AWS Snow
- [X] AWS DMS
- [ ] AWS Connect
- [ ] AWS Glue

### Explicação

**Correta**

AWS DMS - Database Migration Service é um serviço da Web que você pode usar para
migrar dados de bancos de dados on-premises, em uma instância de banco de dados do
Amazon Relational Database Service (Amazon RDS) ou em um banco de dados em uma
instância do Amazon Elastic Compute Cloud (Amazon EC2), para um banco de dados em
um produto da AWS. Esses serviços podem incluir um banco de dados no Amazon RDS
ou em uma instância do Amazon EC2. Também é possível migrar um banco de dados de
um serviço da AWS para um banco de dados on-premises. Você pode migrar entre
endpoints de origem e destino que usam o mesmo mecanismo de banco de dados, como
de um banco de dados Oracle para um banco de dados Oracle. Você também pode
migrar entre endpoints de origem e de destino que usam mecanismos de banco de
dados diferentes, como de um banco de dados Oracle para um banco de dados
PostgreSQL<br>
https:Waws.amazon.com/dms/?nc2=h_ql_prod_mt_dbms

**Incorretas**

AWS Snow - dispositivos portáteis altamente seguros para coletar e processar dados na
borda e migrar dados para dentro e fora da AWS<br>
AWS Glue - é um serviço de integração de dados sem servidor que facilita descobrir,
preparar e combinar dados para análise, machine learning e desenvolvimento da
aplicação<br>
O Amazon Connect é uma central de contatos na nuvem fácil de usar para todos os tipos
de canais, que ajuda você a fornecer um atendimento superior ao cliente a um custo bem
menor. Não confundir com Direct Connect, que é uma solução de serviço de nuvem que
facilita o estabelecimento de uma conexão de rede dedicada entre suas instalações e a
AWS.

#

## Pergunta 12: 

Qual é o serviço da AWS utilizado para migrar banco de dados de forma rápida e segura?

- [ ] AWSSnow
- [X] AWS DMS
- [ ] AWS Connect
- [ ] AWS Glue

### Explicação

**Correta**

AWS DMS - Database Migration Service é um serviço da Web que você pode usar para
migrar dados de bancos de dados on-premises, em uma instância de banco de dados do
Amazon Relational Database Service (Amazon RDS) ou em um banco de dados em uma
instância do Amazon Elastic Compute Cloud (Amazon EC2), para um banco de dados em
um produto da AWS. Esses serviços podem incluir um banco de dados no Amazon RDS
ou em uma instância do Amazon EC2. Também é possível migrar um banco de dados de
um serviço da AWS para um banco de dados on-premises- Você pode migrar entre
endpoints de origem e destino que usam o mesmo mecanismo de banco de dados, como
de um banco de dados Oracle para um banco de dados Oracle. Você também pode
migrar entre endpoints de origem e de destino que usam mecanismos de banco de
dados diferentes, como de um banco de dados Oracle para um banco de dados
PostgreSQL<br>
httpsWaws.amazon.com/d bms

**Incorretas**

AWS Snow - dispositivos portáteis altamente seguros para coletar e processar dados na
borda e migrar dados para dentro e fora da AWS<br>
AWS Glue - é um serviço de integração de dados sem servidor que facilita descobrir,
preparar e combinar dados para análise, machine learning e desenvolvimento da
aplicação<br>
O Amazon Connect é uma central de contatos na nuvem fácil de usar para todos os tipos
de canais, que ajuda você a fornecer um atendimento superior ao cliente a um custo bem
menor. Não confundir com Direct Connect, que é uma solução de serviço de nuvem que
facilita o estabelecimento de uma conexão de rede dedicada entre suas instalações e a
AWS.

#

## Pergunta 13: 

Quais são os 6 pilares do Well-Architected Framework?

- [X] Excelência Operacional, Segurança, Confiabilidade, Desempenho, Eficiente, Otimização de Custos, Sustentabilidade
- [ ] Excelência Operacional, Escalabilidade, Confiabilidade, Desempenho, Eficiente, Otimização de Custos, Disciplina
- [ ] Excelência Operacional, Segurança, Confiabilidade, Desempenho Eficiente, Escalabilidade, Disciplina
- [ ] Excelência Operacional, Segurança, Escalabilidade, Desempenho Eficiente, Otimização de Custos, Sustentabilidade

### Explicação

**Correta**

Os 6 pilares são Excelência Operacional:<br>
- Segurança<br>
- Confiabilidade<br>
- Desempenho<br>
- Eficiente<br>
- Otimização de Custos<br>
- Sustentabilidade (adicionado recentemente).<br>
https://aws.amazon.com/pt/architecture/well-architected/

**Incorretas**

Escalabilidade e Disciplina não são pilares do framework.

#

## Pergunta 14: 

Sua empresa está desenhando uma nova plataforma para distribuição de vídeos em nível
global. Qual é o serviço que pode diminuir a latência entre a requisição e entrega do e entrega do serviço?

- [ ] Amazon ElasticCache
- [ ] Amazon Redis
- [X] Amazon CloudFront
- [ ] Amazon S3

### Explicação

**Correta**

O Amazon CloudFront utiliza a infraestrutura da redes de borda, que estão muito mais
próximas aos usuários finais e podem fazer o cache de conteúdos recorrentes e diminuir
a velocidade de transferência dos dados SQLicitados.<br>
https://aws.amazon.com/pt/cloudfront/

**Incorretas**

O Amazon S3 é a solução para armazenar os arquivos e também pode ser utilizado para
disponibilizar os vídeos através de URLs e acesso públicos aos Buckets, entretanto
podem estar um pouco mais distantes dos usuários finais e ter uma latência um pouco
maior se comparada a utilização dos caches das redes de borda.<br>
O Amazon ElasticCache e Redis são utilizados para armazenar em cache os dados das
aplicações, como consultas mais comuns a banco de dados e arquivos de sessão de
usuário, não para arquivos de vídeos, áudio, etc.

#

## Pergunta 15: 

Qual é o banco de dados NoSql do tipo chave e valor gerenciado pela AWS?

- [ ] Cassandra
- [X] DynamoDB
- [ ] Aurora
- [ ] Mysql

### Explicação

**Correta**

O Amazon DynamoDB é um banco de dados de chave-valor NoSQL, sem servidor e
totalmente gerenciado, projetado para executar aplicações de alta performance em
qualquer escala. O DynamoDB oferece segurança integrada, backups contínuos,
replicação multirregional automatizada, armazenamento em cache na memória e
ferramentas de exportação de dados.
https://aws.amazon.com/pt/dynamodb/?nc2=h_ql_prod_db_ddb

**Incorretas**

Aurora é relacional<br>
MySql é relacional<br>
Cassandra é NoSql, mas não é gerenciado pela AWS.

#

## Pergunta 16: 

Sua empresa fez um contrato para obter um pacote com 50 licenças do Microsoft SQL
Server. Os softwares serão instalados em novos servidores à medida que a empresa
expandir seus negócios ao redor do mundo. A empresa passa por auditorias frequentes e
precisa garantir que só existem softwares licenciados na sua rede. Qual serviço da AWS
facilita essa conformidade?

- [ ] Certificate Manager
- [X] License Manager
- [ ] CloudFormation
- [ ] Config

### Explicação

**Correta**

O AWS License Manager facilita o gerenciamento de suas licenças de software de
fornecedores como Microsoft, SAP, Oracle e IBM em ambientes AWS e on-premises.<br>
O AWS License Manager permite que os administradores criem regras de licenciamento
personalizadas para refletir os períodos de vigência de seus contratos de licenciamento.<br>
Os administradores podem usar essas regras para ajudar a evitar violações de
licenciamento, como o uso de mais licenças do que o estipulado em contrato.

**Incorretas**

O Certificate Manager é utilizado para fornecer segurança de dados em trânsito a partir do SSL/TSL.<br>
O CloudFormation é utilizado para implementar infraestrutura como código.<br>
O Config serve para gerenciar o status e desvios das configurações dos seus serviços.

#

## Pergunta 17: 

Você trabalha num escritório jurídico que lida com um volume muito grande de contratos.
Esses documentos são alterados muitas vezes e requerem um processo de
gerenciamento de versões. Qual serviço da AWS é indicado para armazenar esses
documentos e atender tal requisito?

- [ ] Git
- [X] S3
- [ ] CodeCommit
- [ ] EBS

### Explicação

**Correta**

S3. Ao criar o Bucket para guardar os arquivos, você pode habilitar o versionamento dos
objetos para gerenciar as alterações dos arquivos.<br>
https://aws.amazon.com/pt/s3/features/?nc=sn&loc=2

**Incorretas**

O Git é uma aplicação para realizar o versionamento de arquivos relacionados ao
desenvolvimento de aplicações, geralmente código fonte de desenvolvedores.<br>
O CodeCommit é os serviço da AWS baseado em Git para fazer a gestão de código fonte
de aplicações<br>
O EBS - Elastic Block Store é o serviço utilizado para uso em conjunto do EC2 e para
armazenar dados de aplicações, dados ou para outros usos de computação.

#

## Pergunta 18: 

Na implementação de uma estratégia de backups, qual é número máximo de snapshots
manuais de RDS permitidas por região?

- [ ] 128 por região
- [ ] o número de cópia é virtualmente ilimitado
- [ ] 256 por região
- [X] 100 por região

### Explicação

Para snaphots manuais há uma limitação de 100 por região.<br>
https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/USER_WorkingWit
hAutomatedBackups.html#USER_WorkingWithAutomatedBackups.BackupWindow

#

## Pergunta 19: 

Por que é necessário associar um EBS a uma instância EC2?
APIs
- [ ] Para deixar o fluxo de transmissão de dados mais rápido
- [ ] Para que os dados sejam criptografados
- [X] Para garantira persistência dos dados quando a instância é desligada
- [ ] O Para permitir o armazenamento de uma quantidade maior de dados

### Explicação

Os dados são perdidos sempre que uma instância EC2 é desligada. Trata-se de uma
forma de separar e persistir os dados e de deixar mais econômico e rápido o processo de
AutoScalling.<br>
https://aws.amazon.com/pt/ec2/faqs/

#

## Pergunta 20: 

Sua equipe de desenvolvimento backend começou a utilizar o API Gateway para o
desenvolvimento das novas APIs de um projeto. Quais itens abaixo representam
funcionalidades deste serviço que você irá compartilhar com o time? (Selecione 2)

- [X] criação de APIs RESTfull e WebSocket
- [X] criar, publicar, manter, monitorar APIs
- [ ] Não possui suporte a conteinirização
- [ ] Não possui suporte a funções sem servidor

### Explicação

**Correta**

API Gateway possui suporte a conteinirização e a funções sem servidor.<br>
Amazon API Gateway é um serviço gerenciado que permite que desenvolvedores
criem, publiquem, mantenham, monitorem e protejam APIs em qualquer escala com
facilidade. APIs agem como a "porta de entrada" para aplicativos acessarem dados,
lógica de negócios ou funcionalidade de seus serviços de back-end. Usando o API
Gateway, você pode criar APIs do RESTful e APIs do WebSocket que habilitam
aplicativos de comunicação bidirecionais em tempo real. O API Gateway dá suporte a
cargas de trabalho conteinerizadas e sem servidor, além de aplicativos da web.<br>
https://aws.amazon.com/pt/api-gateway/

**Incorretas**

Se não fosse a palavra '"não" todas as opções estariam corretas.

#

## Pergunta 21: 

Quais dos itens abaixo não fazem parte dos pilares do Well-Architected Framework? (selecione 2)

- [ ] Segurança
- [ ] Excelência Operacional
- [X] Desacoplamento
- [X] Elasticidade

### Explicação

Os pilares são:<br>
- Excelência Operacional<br>
- Segurança<br>
- Confiabilidade<br>
- Performance

Otimização de Custos e Sustentabilidade. Elasticidade e Desacoplamento não fazem
parte dos pilares.<br>
https://aws.amazon.com/architecture/well-architected/?nc2=h_ql_le_wa&wa-lens-
whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.soft-
order=desc

#

## Pergunta 22: 

Como você pode proteger sua conta da AWS contra acessos não autorizados?

- [X] Habilitando a Autenticação Multifator - Multi-Facto Authentication (MFA)
- [ ] Implementando o serviço AWS Cognito
- [ ] Desabilitando o acesso pela AWS ConSQLe
- [ ] Configurando uma segunda senha

### Explicação

**Correta**

A MFA agrega mais segurança porque requer que os usuários para fornecer autenticação
exclusivo de um mecanismo de MFA com suporte da AWS, além das suas credenciais de
login regular ao acessarem sites ou serviços da AWS. É possível utilizar dispositivos
físicos ou virtuais para gerarem o código numérico de 6 dígitos para concluir o login. Ex.
Google Authenticator.<br>
https://docs.aws.amazon.com/pt_br/lAM/latest/UserGuide/id_credentials_mfa.html

**Incorretas**

O Cognito é utilizado para permitir integração com sistema de logins de redes sociais
para aplicações web e mobile. As demais opções são inválidas.

#

## Pergunta 23: 

Qual é a plataforma da AWS para Big Data em Cloud que permite integração com várias
ferramentas de código livre como Apache Spark, Apache Hive, Apache HBase, Apache
Flink, Apache Hudi?

- [ ] Amazon Kinesis
- [ ] Amazon Hadoop
- [ ] Amazon RedShift
- [X] Amazon EMR

### Explicação

**Correta**

O EMR é a solução de big data em nuvem líder do setor para processamento de dados,
análise interativa e machine learning que usa estruturas de código aberto, como Apache
Spark, Apache Hive e Presto<br>
https://aws.amazon.com/emr/?c=a&sec=srv&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc

**Incorretas**

O Haddop é um serviço disponível dentro da plataforma EMR.<br>
O Redshift é um serviço utilizado para BI (Business Inteligence)<br>
O Kinessis é um serviço de transferência de dados em tempo real em streaming de diversos serviços e aplicativos para repositórios da AWS.

#

## Pergunta 24: 

Se você deseja fazer um gerenciamento total do seu banco de dados, qual é o serviço
mais indicado para implementá-lo?

- [ ] DynamoDB
- [ ] DocumentDB
- [ ] RDS
- [X] EC2

### Explicação

**Correta**

EC2 - Se você deseja gerenciar totalmente o banco de dados você precisa instalá-lo
manualmente em servidores físicos.

**Incorretas**

As demais opções são serviços gerenciados pela AWS, que não permitem configuração
laaS.

#

## Pergunta 25: 

Qual é a quantidade atual de regiões disponíveis na infraestrutura global da AWS?

- [ ] 6
- [X] 31
- [ ] 262
- [ ] 81

### Explicação

**31 Regiões** - Em 2023, mas existe estimativa de expansão no futuro.<br>
**99 Zonas de disponibilidade (AZs)** - Em 2023<br>
https://aws.amazon.com/pt/about-aws/global-infrastructure/?nc2=h_ql_le_int_gi

#

## Pergunta 26: 

Você precisa garantir a alta disponibilidade de uma aplicação que será lançada na sua
empresa no Brasil. Qual é a melhor estratégia de uso do AWS RDS para esse requisito?

- [X] Multi A-Z (Distribuir os bancos em mais de uma zona de disponibilidade)
- [ ] O Multi Regions (Distribuir os banco em mais de uma região)
- [ ] O Read Replicas (Utilizar cópias de leitura)
- [ ] O Criar um Security Group para iSQLar apenas os bancos de dados e aumentar a performance

### Explicação

Multi A-Z - https://aws.amazon.com/rds/features/read-replicas/<br>
Multi Region é indicado pra DR<br>
Read Replicas pra aliviar gargalos de leitura<br>
Security Group protege mas não aumenta a disponibilidade<br>

#

## Pergunta 27: 
A AWS obtém regularmente, a validação de terceiros para milhares de requisitos globais
de conformidade para ajudá-la a atender aos padrões de segurança e conformidade.
Com o seu uso, você herda os controles de segurança mais recentes, fortalecendo seus
próprios programas de conformidade e certificação. Para quais padrões de segurança e
certificações a AWS oferece suporte? (selecione 2 alternativas)

- [ ] GDPR, FIPS 140-2 e NTFS-BBI
- [X] PCI-DSS, HIPAA/HITECH, FedRAMP
- [X] GDPR, FIPS 140-2 e NIST 800-171
- [ ] PCI-DSS, HIPAA/HITECH, CFLOI

### Explicação

**Correta**

PCI-DSS, HIPAA/HITECH, FedRAMP, GDPR, FIPS 140-2 e NIST 800-171<br>
https://aws.amazon.com/pt/security/

**Incorretas**

Nas outras opções tem NTFS-BBI, CFLOI, é importante ficar atento em alguns detalhes
neste tipo de questão.

#

## Pergunta 28: 

Qual é o modelo de planos flexíveis que oferece preços mais baixos em comparação com
os preços sob demanda, em troca de um compromisso de uso específico (medido em
USD/hora) por um período de um ou três anos?

- [ ] AWS Efficient cost
- [X] Savings Plans
- [ ] Low Cost
- [ ] AWS Billing

### Explicação

Saving Plans - https://aws.amazon.com/pt/savingsplans/

#

## Pergunta 29: 
Qual é a maior diferença entre os serviços AWS RDS e DynamoDB?

- [ ] RDS é NoSQL, DynamoDB é SQL
- [ ] Nenhuma das opções
- [ ] RDS é totalmente gerenciado, DynamoDB não é gerenciado
- [X] RDS é SQL, DynamoDB é NoSQL

### Explicação

**Correta**

RDS é SQL, DynamoDB é NoSQL

#

## Pergunta 30: 

Sua empresa deseja implementar governança nos serviços de Tl que estejam aprovados
para uso na AWS acompanhando o custo, desempenho, segurança e status operacional
dos mesmos. Qual é o serviço que permite a criação de catálogos de serviços de Tl para
essa finalidade?

- [ ] AWS IT Service
- [ ] AWS Catalog
- [X] AWS Service Catalog
- [ ] AWS Console Manager

### Explicação

**Correta**

AWS Service Catalog
https://aws.amazon.com/pt/servicecatalog/?aws-service-catalog.sort-
by=item.additionalFields.createdDate&aws-service-catalog.sort-order=desc

**Incorretas**

AWS Catalog e IT service não são serviços disponíveis na AWS<br>
AWS Console Manager é a interface web utilizada para gerenciar todos os serviços disponíveis.

#

## Pergunta 31: 

Sua empresa está analisando o banco de dados DynamoDB para conhecer
oportunidades em seu uso. Qual opção abaixo **não** é uma característica do serviço?

- [ ] É um banco de dados sem servidor
- [X] É um banco de dados cobrado por MB na solicitação de gravação e leitura
- [ ] É um banco de dados totalmente gerenciado
- [ ] É um banco de dados de valores-chave e documentos

### Explicação

**Correta**

O DynamoDB é um banco de dados não relacional, sem servidor, totalmente gerenciado
pela AWS, não possui esquema e é baseado em tabelas compostas por colunas de chave
x valor. Pode ser utilizador para guardar dados não estruturados no formato Json e
documentos.<br>
https://aws.amazon.com/pt/dynamodb/?nc2=type_a

**Incorretas**

Definição de preço é por unidade de gravação e leitura por KB.
https://aws.amazon.com/pt/dynamodb/pricing/on-demand/

#

## Pergunta 32: 
Sobre o AWS Budget e suas finalidades podemos afirmar que: (Selecione 3 alternativas)

- [X] Podem ser utilizados para enviar alertas para te ajudar no controle do uso dos serviços da sua conta
- [X] Podem ser usados para criar e gerenciar orçamentos
- [ ] Podem enviar notificações para até 5 destinatários por email
- [X] Podem ser usados para refinar e filtrar orçamentos

### Explicação

O serviço tem todas as finalidades acima, entretanto pode enviar e-mail para até 10
destinatários por notificação/alerta e não 5.<br>
https://aws.amazon.com/pt/aws-cost-management/aws-budgets/

#

## Pergunta 33: 

Sua empresa começou a utilizar o ECS e conteinerizou 2 microsserviços de uma
aplicação que possuem cargas de trabalho diferentes ao longo dia. O primeiro tem mais
acessos durante a manhã e o segundo tem mais acesso à tarde, invertendo o cenário no
consumo de recursos. Qual solução você deve adotar para que esses serviços escalem
de forma automática para otimizar o uso dos recursos da sua infraestrutura?

- [X] EKS
- [ ] Lambda
- [ ] O ECR
- [ ] O EC2

### Explicação

**Correta**

EKS - Kubernetes - Para orquestrar os conteiners<br>
https://aws.amazon.com/eks/?c=cn&sec=srv&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc&eks-
blogs.sort-by=item.additionalFields.createdDate&eks-blogs.soft-order=desc

**Incorretas**

ECR - Docker Conteiner Registry - é um registro de contêineres do Docker totalmente
gerenciado que permite que desenvolvedores armazenem, gerenciem e implantem
facilmente imagens de contêineres do Docker.<br>
EC2 - Elastic Compute Cloud - é um serviço Web que disponibiliza capacidade
computacional segura e redimensionável na nuvem.<br>
Lambda - é um serviço de computação sem servidor que permite executar código sem
provisionar ou gerenciar servidores, criando lógica de dimensionamento de cluster com
reconhecimento de workloads, mantendo integrações de eventos ou gerenciando
tempos de execução

#

## Pergunta 34: 
Qual é o serviço utilizado para executar containers sem servidores e diminuir a
necessidade dos desenvolvedores se preocuparem com questões relacionadas ao
gerenciamento de instâncias e infraestrutura?

- [ ] EKS
- [ ] ECS
- [X] Fargate
- [ ] Lambda

### Explicação

**Correta**

O AWS Fargate é um mecanismo de computação sem servidor e com pagamento
conforme o uso que permite a você se concentrar em construir aplicações sem gerenciar
servidores. <br>
O AWS Fargate é compatível com o serviço de container ECS (Elastic
Container Service) e com o orquestrador de container EKS (Elastic Kubernetes Services).<br>
O Fargate acaba com a necessidade de ser proprietário, executar e gerenciar o ciclo de
vida de uma infraestrutura de computação, para que você possa se concentrar nas suas
aplicações.<br>
https://aws.amazon.com/pt/fargate/

**Incorretas**

Apesar do ECS e EKS fornecerem serviços para conteiner, é o Fargate que fornece os
recursos para rodar numa arquitetura sem servidor<br>
https://aws.amazon.com/fargate/?c=ser&sec=srv&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc&fargate-
blogs.sort-by=item.additionalFields.createdDate&fargate-blogs.sort-order=desc<br>
Lambda é utilizado para funções sem servidores, não conteiners

#

## Pergunta 35: 

A Amazon oferece várias classes de armazenamento no S3 específicas para cada tipo de
uso. Qual das opções abaixo são classes existentes no serviço? (selecione 3)

- [ ] S3 Enterprise
- [X] S3 Intelligent-Tiering
- [X] S3 Standard
- [X] S3 Standard Infrequent Access
- [ ] S3 Business

### Explicação

Essas são três das sete classes existentes:<br>
- S3 Standard, para armazenamento geral de dados acessados com frequência<br>
- S3 Intelligent-Tiering, para dados com padrões de acesso desconhecidos ou variáveis,<br>
- S3 Standard-lnfrequent Access (S3 Standard — IA)<br>
- S3 One Zone-lnfrequent Access (S3 One Zone — IA) para dados duradouros acessados com menos frequência e Amazon<br>
- S3 Glacier (S3 Glacier)<br>
- S3 Glacier Deep Archive (S3 Glacier Deep Archive) para preservação digital e arquivamento de longo prazo.<br>
- S3 Outposts para armazenar seus dados do S3 on-premises<br>
https://aws.amazon.com/s3/storage-classes/?nc=sn&loc=3

#

## Pergunta 36: 

Sua empresa começou a usar a AWS e precisa liberar os acessos para 100 pessoas. Uma
vez que o time é composto por desenvolvedores, dbas e arquitetos, e que cada time
precisa de um acesso exclusivo a determinados recursos, qual serviço você utilizará para
otimizar essa gestão?

- [X] IAM Grupos
- [ ] Cognito
- [ ] Organizations
- [ ] IAM Team

### Explicação

**Correta**

Com o AIM Grupos você pode criar um grupo para cada time, liberar os acessos aos
recursos ao grupo e ir incluir cada pessoa ao respectivo grupo, isso permite que novos
colaboradores sejam cadastrados de uma forma bem mais dinâmica

**Incorretas**

IAM Team não é um serviço válido na AWS.<br>
O Gognito é um serviço para ser utilizado em processos de login e autenticação de
aplicações web e mobile, permitindo a integração com logins de midias sociais como
Apple, Google, Facebook, etc.<br>
O Organizations é um serviço utilizado para integrar diversas contas da AWS permitindo
a integração entre os serviços e também a consolidação de custos.

#

## Pergunta 37: 
Qual é o serviço capaz de coletar e processar, em tempo real, um grande volume de
streams de dados oriundos de diversos dispositivos, gerando novas informações para
rápidas reações e direções?

- [ ] SNS
- [ ] SQS
- [X] Kinesis
- [ ] EventBridge

### Explicação

**Correta**

O Amazon Kinesis facilita a coleta, o processamento e a análise de dados de streaming
em tempo real, permitindo que você obtenha insights oportunos e reaja rapidamente às
novas informações. O Amazon Kinesis oferece recursos essenciais para processar dados
de streaming em qualquer escala de forma econômica, além da flexibilidade de escolher
as ferramentas mais adequadas aos requisitos dos aplicativos. Com o Amazon Kinesis,
você pode consumir dados em tempo real como vídeo, áudio, logs de aplicativos,
clickstreams de sites e dados de telemetria de IOT para machine learning, análises e
outros aplicativos. O Amazon Kinesis permite processar e analisar dados assim que são
recebidos e responder instantaneamente, em vez de aguardar a conclusão da coleta de
dados para poder iniciar o processamento.<br>
https://aws.amazon.com/kinesis/?nc2=h_ql_prod_an_kin

**Incorretas**

SNS - O Amazon Simple Notification Service é um serviço de mensagens totalmente
gerenciado para a comunicação de aplicação para aplicação (A2A) e de aplicação para
pessoa (A2P).A funcionalidade pub/sub de A2A fornece tópicos para sistemas de
mensagens de alta taxa de transferência baseados em push e de muitos para muitos
entre sistemas distribuídos, microsserviços e aplicativos sem servidor orientados por
eventos.<br>
SQS - O Amazon Simple Queue Service é um serviço de filas de mensagens gerenciado
que permite o desacoplamento e a escalabilidade de microsserviços, sistemas
distribuídos e aplicações sem servidor<br>
EventBridge - O Amazon EventBridge é um barramento de eventos sem servidor que
torna mais fácil a criação de aplicações orientadas por eventos em escala usando
eventos gerados com base em suas aplicações, aplicações integradas de software como
serviço (SaaS) e serviços da AWS.

#

## Pergunta 38: 

Qual banco de dados foi projetado para oferecer disponibilidade superior a
replicando seis cópias dos seus dados em três zonas diferentes e fazendo o backup
continuo de seus dados no Amazon S3?

- [ ] Mysql
- [X] Aurora
- [ ] DynamoDB
- [ ] MariaDB

### Explicação

**Correta**

Aurora - https://aws.amazon.com/pt/rds/aurora/?nc2=h_ql_prod_fs_aa&aurora-whats-new.sort-
by=item.additionalFields.postDateTime&aurora-whats-new.soft-order=desc

**Incorretas**

Os demais bancos não possuem essas características.

#

## Pergunta 39: 

Seus clientes da Europa e da Austrália estão reclamando que o seu site está demorando
muito para carregar as imagens, proporcionando a eles uma experiência muito ruim. Uma
vez que você utiliza a sua infraestrutura na Região de São Paulo, o que você poderia
fazer, imediatamente, para melhorar esse cenário?

- [ ] habilitar o Intelligent-Tiering das classes do S3
- [X] habililitar o CloudFront
- [ ] criar uma conta nessas regiões e duplicar a infraestrutura
- [ ] deixar as imagens numa resolução bem baixa

### Explicação

**Correta**

CloudFront faz o cache do conteúdo numa edge location (infraestrutura de borda, que
são data centers mais próximos dos usuários, mas que não podem ter implementações
diretas de serviços pelos clientes, apenas para melhorias de performance e conexões)
https://aws.amazon.com/cloudfront/?nc2=h_ql_prod_nt_cf

**Incorretas**

O Intelligent-Tiering das classes do S3 movimenta objetos entre as classe do S3
permitindo o melhor uso do armazenamento e melhor gestão de custos. Como a
reclamação vem de clientes de determinadas regiões, o problema parece não estar
relacionado ao S3 e sim a velocidade que o conteúdo chega a determinados usuários.<br>
As demais implementações não são rápidas e nem baratas pois requerem ajuste na
infraestrutura, aplicação ou no conteúdo.

#

## Pergunta 40: 

Uma das grandes vantagens no uso da AWS está nas formas de pagamentos dos seus
serviços. Qual é forma de pagamentos padrão utilizada na maior parte dos seus
serviços?

- [X] Pagamento conforme o uso
- [ ] Pagamento conforme o contrato
- [ ] Pagamento conforme o licenciamento
- [ ] Pagamento conforme a compra

### Explicação

Pagamento conforme o uso.<br>
https://aws.amazon.com/pt/pricing/?nc2=h_ql_pr_ln
(Correto)

#

## Pergunta 41: 

No modelo de responsabilidade compartilhada, a AWS deve proteger todos os dados
trafegados na sua infraestrutura global. Sobre a criptografia realizada neste processo,
podemos afirmar que:

- [X] O AWS criptografa automaticamente os dados na camada física antes de sair de suas instalações protegidas
- [ ] AWS criptografa automaticamente os dados na camada lógica antes de sair de suas instalações protegidas
- [ ] O AWS não criptografa os dados, entretanto fornece o KMS para o usuário fazê-la
- [ ] O AAWS não criptografa os dados, entretanto fornece o AWS Certificate Manager para o usuário fazê-la

### Explicação

Criptografia na camada física<br>
https://aws.amazon.com/pt/security/

#

## Pergunta 42: 

Você está dando consultoria para uma pequena empresa que deseja disponibilizar um
site dinâmico em WordPress e com custo mínimo. Qual dos serviços abaixo oferece um
servidor privado virtual simples (VPS) de baixo custo e que pode atender essa
necessidade?

- [ ] Amazon ECS
- [ ] Amazon EC2
- [X] Amazon LightSail
- [ ] Amazon S3

### Explicação

**Correta**

O WordPress é um sistema livre e aberto de gestão de conteúdo para internet, baseado
em PHP com banco de dados MySQL, executado em um servidor e o Amazon LightSail é
a solução ideal pra ele.<br>
https://aws.amazon.com/pt/lightsail/?nc2=h_ql_prod_fs_ls

**Incorretas**

O EC2 pode ser utilizado para o hospedar o site, porém não é a solução mais barata.<br>
O S3 permite a implementação de um site estático, que não é o caso do WordPress<br>
O ECS é utilizado para a implementação de containars, que não é a arquitetura existente no WordPress.

#

## Pergunta 43: 

Qual é o modelo de utilização de cloud onde não é necessário se preocupar com o
gerenciamento dos recursos de infraestrutura de tecnologia, permitindo que o foco do
cliente seja, principalmente, no desenvolvimento das aplicações que vão ser executados
sobre os recursos?

- [ ] BaaS
- [ ] SaaS
- [X] IaaS
- [ ] PaaS

### Explicação

**Correta**

PaaS - Plataforma como serviço.<br>
https://aws.amazon.com/what-is-cloud-computing/?nc2=h_ql_le_int_cc

**Incorretas**

laaS - Infraestrutura como serviço requer que os softwares de base, como sistemas
operacionais, softwares de bancos de dados, entre outros, sejam gerenciados pelo
próprio cliente.<br>
SaaS - Software como serviço não requer nenhuma construção, é uma solução pronta
para o uso.<br>
BaaS - Backend como serviço requer uma construção parcial, a construção é apenas no
Frontend.<br>

#

## Pergunta 45: Incorreto
Qual é o serviço, que através da infraestrutura global da AWS, pode ser utilizado quando
as suas aplicações apresentarem problemas de tráfego devido ao congestionamento da
Internet?

- [ ] AWS Snowball
- [X] AWS Global Accelerator
- [ ] AWS CloudFront
- [ ] AWS DataSync

### Explicação

**Correta**

O AWS Global Accelerator é um serviço de redes que melhora a performance do tráfego
de seus usuários em até 60%. Quando a Internet está congestionada, otimiza o caminho
para sua aplicação manter a perda de pacotes, o jitter e a latência consistentemente
baixos. Fornece IPS estáticos como pontos únicos de entrada para a otimização da
performance.<br>
https://aws.amazon.com/pt/global-accelerator/?blogs-global-accelerator.sort-
global-accelerator-wn.sort-by=item.additionalFields.postDateTime&aws-global-
accelerator-wn.soft-order=desc

**Incorretas**

O Snowball é um dispositivo físico para migrar grandes quantidade de dados entre data
centers.<br>
O AWS CloudFront é utilizado para fazer cache de conteúdo mais próximo ao usuário,
reduz problema de latência e é recomendado para conteúdos reaproveitáveis, não
resolveria questões associados a tráfego de dados dinâmicos associados a
congestionamento na Internet.<br>
O AWS DataSync é utilizado para automatizar e otimizar processos de sincronização de
dados entre Data Centers.

#

## Pergunta 46: 
Você construiu uma aplicação no EC2 que se conecta aos dados no RDS. Qual serviço
você deve utilizar para que as devidas configurações de acesso entre a aplicação e o
banco de dados sejam realizadas?

- [ ] IAM Users
- [X] IAM Roles
- [ ] IAM Groups
- [ ] IAM Grant

### Explicação

**Correta**

O IAM Roles é o serviço utilizado para gerenciar os acessos que as aplicações podem
receber. Uma aplicação sempre vai possuir uma Role para acessar algum serviço.<br>
https://aws.amazon.com/iam/features/manage-roles/

**Incorretas**

O IAM Users é utilizado para gerenciar os usuários da sua conta.<br>
O IAM Groups é utilizado para agrupar usuários da sua conta.<br>
O IAM Grant não é um serviço existente na AWS.

#

## Pergunta 47: 

Qual serviço é utilizado para logar as ações dos seus usuários dentro da AWS?

- [ ] S3
- [X] CloudTrail
- [ ] CloudWatch logs
- [ ] O IAM

### Explicação

**Correta**

CloudTrail pode logar todas as ações dos usuário, muito utilizada para auditorias na
infraestrutura da AWS.

**Incorretas**

O CloudWatch logs é utilizado para armazenar a log de métricas de monitoramento de serviços e logs de observabilidade de aplicações.<br>
O S3 é utilizado para armazenar arquivos de forma geral<br>
O IAM é utilizado para fazer o gerenciamento de acessos de usuários, grupos de usuários e aplicações

#

## Pergunta 48: 

Algumas aplicações críticas da sua empresa começaram a apresentar erros e, por falta
de logs, a equipe de suporte está tendo dificuldade na resolução dos problemas. Qual
serviço da AWS você recomendaria para monitorar o ambiente e coletar as logs?

- [X] AWS CloudWatch
- [ ] AWS Monitor
- [ ] AWS CloudTrail
- [ ] AWS Log

### Explicação

**Correta**

O Amazon CloudWatch é um serviço de monitoramento e observabilidade criado para
engenheiros de DevOps, desenvolvedores, engenheiros de confiabilidade de sites
(SREs), gerentes de Tl e proprietários de produtos. O CloudWatch fornece dados e
insights úteis para monitorar suas aplicações, responder às mudanças de performance
de todo o sistema e otimizar a utilização de recursos. O CloudWatch coleta dados
operacionais e de monitoramento na forma de logs, métricas e eventos.<br>
https://aws.amazon.com/pt/cloudwatch/?nci=h_ls

**Incorretas**

AWS CloudTrail é utilizado para logar as ações em APIs de serviços da AWS como
Start/Stop de uma instância EC2, entre outros.<br>
AWS Monitor e Log não existem.<br>

#

## Pergunta 49: 

No modelo de Responsabilidade Compartilhada, qual é o papel da AWS? (selecione 2 alternativas)

- [ ] Atualizar o Sistema Operacional das Instâncias EC2
- [ ] Proteger o acesso aos dados das aplicações dos usuários
- [X] Fazer a manutenção dos hardware
- [X] Proteger o data center

### Explicação

É importante entender quais são as responsabilidade da AWS e quais são as
responsabilidades do cliente neste modelo. Para mais detalhes leia a documentação
deste link<br>
https://aws.amazon.com/pt/compliance/shared-responsibility-model/

#

## Pergunta 50: 

Qual dos seguintes ítens é de responsabilidade exclusiva da AWS no modelo de
responsabilidade compartilhada (shared responsability model)?

- [X] Proteger a infraestrutura global
- [ ] Gerenciar imagens customizadas das instâncias do AMI
- [ ] Atualizar patch de segurança em instâncias do clientes
- [ ] Proteger os dados das aplicações dos usuários

### Explicação

**Correta**

No modelo de responsabilidade compartilhada, todos os itens de infraestrutura são de
responsabilidade exclusiva da AWS, Manutenção de hardware, segurança do data center,
garantia do fornecimento de energia, etc.<br>
https://aws.amazon.com/pt/compliance/shared-responsibility-model/

**Incorretas**

Atualizar patch de segurança em instâncias do clientes, Proteger os dados das
aplicações dos usuários, Gerenciar imagens customizadas das instâncias do AMI podem
ser de responsabilidade de ambas as partes, AWS e Cliente.

#

## Pergunta 51: Incorreto
Sua empresa precisa executar centenas de batch para atualizar diversas informações
dos seus clientes sem ter a dimensão dos recursos tecnológicos que precisará utilizar,
qual é a melhor solução a ser utilizada?

- [ ] AWS EC2 Reserved
- [X] AWS Batch
- [ ] AWS Step Functions
- [ ] AWS OnDemand

### Explicação

**Correta**

AWS Batch - https://aws.amazon.com/batch/?nc2=h_ql_prod_cp_ba

**Incorretas**

O AWS Step Functions é um serviço de fluxo de trabalho visual que utiliza pouco código,
usado para orquestrar serviços da AWS, automatizar processos de negócios e criar
aplicações sem servidor. Os fluxos de trabalho gerenciam falhas, novas tentativas,
paralelização, integrações de serviços e observabilidade, de modo que os
desenvolvedores possam se concentrar na lógica de negócios com maior valor.<br>
https://aws.amazon.com/pt/step-functions/?nc2=type_a&step-functions.sort-
by=item.additionalFields.postDateTime&step-functions.sort-order=desc<br>
Reserved e OnDemand são forma de uso e pagamento de serviços de computação em
nuvem.

#

## Pergunta 52: 

Qual plano de suporte oferece o AWS Trusted Advisor, serviço que fornece
recomendações para ajudar na utilização das melhores práticas de uso?

- [ ] Business
- [ ] Enterprise
- [ ] Developer
- [X] Todos

### Explicação

Todos os planos oferecem esse serviço.

A diferença é que no plano básico e Developer são liberados 7 checagens de
recomendações, enquanto nos demais planos são liberados todas as checagens e
verificações de recomendações.<br>
https://aws.amazon.com/premiumsupport/plans/

#

## Pergunta 53: 
Sua empresa precisa implementar a integração rápida entre escritórios em São Paulo,
Moscow e 2 mil funcionários ao redor do mundo. Qual é o serviço da AWS que permite
realizar essa integração de forma ágil e escalável?

- [ ] AWS DataSync
- [X] AWS VPN
- [ ] AWS Link
- [ ] AWS VPC

### Explicação

**Correta**

AWS VPN (permite acesso remoto) - https://aws.amazon.com/pt/vpn/?nc2=h_ql_prod_nt_avpn

**Incorretas**

O VPC - Virtual Private Cloud é utilizada para fornecer uma rede privada isolada para
alocar diversos serviços da AWS de sua conta.<br>
O AWS DataSyn é utilizado para fazer cópias de dados de sua infraestrutura on premise
para a AWS de forma automatizada.<br>
O AWS Link não é um serviço existente na AWS.

#

## Pergunta 54: 
Qual serviço pode ser utilizado para explorar todos os custos dos recursos utilizados na
AWS?

- [ ] AWS Price
- [ ] AWS Pricing Calculator
- [ ] AWS Budget
- [X] AWS Cost Explorer

### Explicação

**Correta**

AWS Cost Explorer permite visualizar, entender e gerenciar os custos e o uso de todos os
recursos da AWS ao longo do tempo. E possível ver o detalhe do consumo de cada
serviço ao longo do tempo.<br>
https://aws.amazon.com/aws-cost-management/aws-cost-explorer/

**Incorretas**

AWS Pricing Calculator é utilizado para estimar custos<br>
AWS Budget - O Orçamentos da AWS permite que você defina orçamentos
personalizados que enviam alertas quando o uso ou os custos excedem (ou tendem a
exceder) o valor orçado<br>
AWS Price não é um serviço disponível na AWS<br>

#

## Pergunta 55: 

Quais são as principais funções do AWS Glue? (Selecione 3 alternativas)

- [X] Extrair dados
- [X] Carregar dados
- [ ] Arquivar dados
- [ ] Criptografar dados
- [X] Transformar dados

### Explicação

Corretas

É um serviço indicado para ETL (Extract, Transform, Load). O AWS Glue é um serviço de
integração de dados com tecnologia sem servidor que facilita a descoberta, preparação,
movimentação e integração de dados de várias fontes para análise, machine learning
(ML) e desenvolvimento de aplicações.<br>
https://aws.amazon.com/pt/glue/

**Incorretas**

Para criptografar dados é recomendado o uso de chaves fornecidas pelo AWS KMS.<br>
Para arquivar dados como objetos é recomendado o uso do S3.

#

## Pergunta 56: Correto
Qual fator é considerado para calcular o Total Cost of Ownership (TCO) numa migração
para a AWS?

- [ ] O número de Certificado de Segurança
- [ ] O número de APIs
- [X] O número de servidores
- [ ] O número de usuários

### Explicação

O número de servidores, o custo da AWS sempre é baseado nos itens de infraestrutura
que suportam os serviços, como computação, armazenamento e redes.

**Incorretas**

O número de usuários, APIs e certificados de segurança, por si só, não são suficientes
para fazer uma estimativa de custo que é baseada em processamento e consumo da
infraestrutura.

#

## Pergunta 57: 

Qual é o banco de dados sem servidor (serverless) ofertado pela AWS?

- [ ] Mysql
- [ ] Aurora
- [ ] MariaDB
- [X] DynamoDB

### Explicação

**Correta**

O Amazon DynamoDB é um banco de dados de chave-valor NoSQL, sem servidor e
totalmente gerenciado, projetado para executar aplicações de alta performance em
qualquer escala.<br>
https://aws.amazon.com/pt/dynamodb/

**Incorretas**

Os demais bancos de dados são do tipo relacional e requerem a implementação através
do RDS ou instalação em instâncias EC2.<br>
Outra opção que seria possível e o Aurora Serverless, que não está na lista.

#

## Pergunta 58: Incorreto
Quais dos seguintes serviços ajudam a sua aplicação a escalar baseado em demanda? (Escolha 2)

- [X] ELB
- [X] Auto Scaling
- [ ] CloudFront
- [ ] CloudFormation
- [ ] Route53

### Explicação

**Corretas**

Auto Scaling permite que configurações sejam feitas para manter o processo de
escalonamento automático, garantindo que sua aplicação sempre tenha o número ideal
de instâncias para atender a sua carga de trabalho com a melhor otimização de recursos
possível.<br>
O ELB permite que o tráfego seja distribuído entre as máquinas escalonadas.
https://aws.amazon.com/autoscaling/?nc2=type_a

#

## Pergunta 59: 
Qual é a melhor prática para atender o princípio: "construa para falhar e nada irá falhar"?

- [ ] Utilizar CloudFront para fazer o cache do conteúdo
- [X] Implantar a aplicação em múltiplas zonas de disponibilidade
- [ ] Monitorar o ambiente pare enviar alertas com o CloudWatch
- [ ] Implantar a aplicação sempre com o CodeDeploy

### Explicação

**Correta**

Distribuir a carga em mais de uma zona de disponibilidade aumenta consideravelmente a
disponibilidade da aplicação. Se uma falhar, as outras devem estar preparadas para
manter os serviços.<br>
Independente da plataforma que utilizamos, quanto mais tivermos a mentalidade de que
alguma peça pode falhar, mais pensaremos em maneiras de contornar essa falha.

**Incorretas**

O CloudWatch é utilizado para monitoramento e observabilidade das aplicações.<br>
O CloudFront aumenta a performance para o usuário final.<br>
O CloudDeploy é utilizado para implantar as aplicações.<br>

#

## Pergunta 60: Correto
Qual serviço da AWS deve ser usado se você deseja configurar alarme de cobrança? (AWS billing alarm)

- [ ] CloudTrail
- [X] CloudWatch
- [ ] CloudBilling
- [ ] CloudMonitor

### Explicação

**Correta**

O CloudWatch permite que os serviços sejam monitorados para envio de mensagens e
alarmes, inclusive é utilizado no AWS Budget para enviar alertas de orçamento
estourado.

**Incorretas**

O CloudTrail é utilizado para logar ações de usuários em APIs de serviços.<br>
O CloudMonitor e CloudBilling não existem.<br>

#

## Pergunta 61: 

Sua empresa recentemente foi auditada e autuada, pois mantinha arquivos com dados
sensíveis do cliente expostos na sua rede interna, colocando em risco a imagem do
cliente e da empresa. Qual serviço da AWS pode ser utilizado para monitorar os dados e
evitar esse tipo de ocorrência?

- [ ] AWS GuardDuty
- [ ] AWS KMS
- [ ] AWS Sensitive
- [X] AWS Macie

### Explicação

**Correta**

AWS Macie é um serviço de segurança e privacidade de dados totalmente gerenciado
que usa machine learning e correspondência de padrões para descobrir e proteger seus
dados confidenciais na AWS<br>
https://aws.amazon.com/macie/?nc2=h_ql_prod_se_ma

**Incorretas**

AWS GuardDuty é um serviço de detecção de ameaças que monitora continuamente
atividades mal-intencionadas e comportamentos não autorizados para proteger suas
contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.<br>
AWS KMS - Key Management Service - facilita a criação e o gerenciamento de chaves
criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em
seus aplicativos.AWS Sensitive não é um serviço que existe na AWS.<br>

#

## Pergunta 62: 

Qual serviço que é totalmente gerenciado pela AWS e que faz parte da arquitetura da
esteira de integração contínua que compila, testa e cria pacotes para a implantação?

- [ ] AWS Pipeline
- [ ] AWS CodeDeploy
- [X] AWS CodeBuild
- [ ] AWS CodeCommit

### Explicação

**Correta**

O AWS CodeBuild é um serviço de integração contínua totalmente gerenciado que
compila o código-fonte, realiza testes e produz pacotes de software prontos para
implantação. Com o CodeBuild, você não precisa provisionar, gerenciar e escalar seus
próprios servidores de compilação. O CodeBuild escala continuamente e processa
múltiplas compilações ao mesmo tempo, o que evita que elas fiquem esperando em uma
fila. Você pode começar a usar rapidamente com ambientes de compilação pré-definidos
ou criar ambientes de compilação personalizados com suas próprias ferramentas de
compilação.<br>
https://aws.amazon.com/pt/codebuild/

**Incorretas**

AWS CodeCommit é o serviço para gerenciar o código<br>
AWS CodeDeploy é o serviço utilizado para implantar e distribuir o código em algum
serviço, instâncias EC2, S3, etc.<br>
AWS Pipeline, não existe. AWS CodePipeline que existe e é utilizado para montar a
esteira que integra todos esses serviços fornecendo funções de CI/CD para o
desenvolvimento.

#

## Pergunta 63: 

Qual é o serviço da AWS que oferece diversos tipos de máquinas com capacidades
computacionais para atender a diversas necessidades de cargas de trabalho (workloads)?

- [X] EC2
- [ ] S3
- [ ] EBS
- [ ] EFS

### Explicação

**Correta**

EC2 - Elastic Compute Cloud oferece a plataforma de computação mais ampla e
profunda, com mais de 500 instâncias e opções de processador, armazenamento, redes,
sistema operacional e modelo de compra mais recentes para te ajudar a atender melhor
às necessidades da sua workload - https://aws.amazon.com/pt/ec2/

**Incorretas**

S3 é o serviço padrão para armazenar arquivos e metadados dos mesmos como objetos
em buckets<br>
EBS é o serviço utilizado como storage para diversas funcionalidades em complemento
ao EC2, como instalação de banco de dados IAAS, entre outras.<br>
EFS é o Elastic File System que pode ser utilizado para fornecer sistema de arquivos
para uma ou mais instâncias EC2

#

## Pergunta 64: 
Qual é o formato de arquivo utilizado na maioria das configurações de serviços da AWS?

- [ ] XML
- [ ] TXT
- [ ] Config
- [X] JSON

### Explicação

O JSON é utilizado na maior parte dos serviços, outro arquivo utilizado também é o YAML
pra templates do Cloud Formation

#

## Pergunta 65: 

Quais são as regras para a criação de nome de Bucket do S3? (Selecione 3)

- [X] Devem consistir apenas em letras minúsculas, números, pontos (.)e hífens (-)
- [X] Devem começar e terminar com uma letra ou um número
- [ ] Devem ser formatados como um endereço IP sempre que possível
- [X] Devem possuir de 3 a 63 caracteres

### Explicação

Os Buckets não devem ser formatados como um endereço IP<br>
https:Wdocs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html








