# Simulado AWS Cloud Practitioner 1/5
## Pergunta 1: 
Qual serviço da AWS possui um catálogo onde os clientes podem encontrar aplicações
desenvolvidas porterceiros, prontas para serem instaladas e executadas para atender as
mais diversas necessidades de neçõcio?

- [ ] AWS AMI
- [X] AWS Marketplace
- [ ] AWS MFA
- [ ] AWS OpsWorks

### Explicação

**Correta**

AWS Marketplace

Existem muitos tipos de aplicações e contextos de neçõcio para uso imediato.

Útil para comercializar alguma aplicação feita pelo cliente.

Essa pergunta é direta, porém, é importante pensar se poderia entrar em contextos onde
a sua empresa tem a necessidade de comprar alguma aplicação pronta para atender
alguma finalidade latente e especifica, cuja compra seja melhor que o desenvolvi mento.
https•Waws-amazon.com/marketpIace/?nc2=type_a

**Incorretas**

O AWS MFA - Multi Factor Authentication adiciona uma camada a mais no processo de
autenticação no login pelo ConSQLe

O AWS AMI - Amazon Machine Images (AWS) são pré-configuraçaes de uma lista de
sistemas operacionais para a instalação instantânea em instâncias EC2

O AWS OpsWorks é um serviço de gerenciamento de configurações que oferece
instâncias gerenciadas do Chef e do Puppet. O Chef e o Puppet são plataformas de
automação que permitem usar cód igo para automatizar a configuração de servidores.

O OpsWorks permite usar o Chef e o Puppet para automatizar a forma como os servidores
são configurados, implantados e gerenciados em instâncias do Amazon EC2 ou
ambientes de computação no local

#
## Pergunta 2: 
O time de segurança da informação da sua empresa classificou seu site com alto risco de
exposição de dados sensíveis, as mensagens trocadas entre os usuários e os servidores
não estão sendo criptografados. Qual serviço pode auxiliar no reparo deste problema?

- [X] AWS Certificate Manager
- [ ] AWS IAM
- [ ] AWS KMS
- [ ] AWS Cognito
### Explicação

**Correta**

O AWS Certificate Manager permite a criação e gerenciamento de certificados digitais
que são utilizados para criptografar os dados entre os usuários e os servidores com base
no protocolo https tornando o tráfego de dados seguro. Quando certificados digitais não
são utilizados, dados de usuários, senhas, números de documentos e cartões de crédito,
etc são trafegados sem nenhuma segurança e podem ser expostos de forma indevida.
https://aws.amazon.com/certificate-manager/?nc2=type_a

**Incorretas**

AWS Cognito é um serviço que pode ser utilizado para fazer controle de acesso em
aplicações web e mobile, ofertando diversas funcionalidades para esse fim.<br>
AWS IAM é o serviço utilizado para gerenciar acesso de usuário e serviços.<br>
AWS KMS é o serviço utilizado para criar chaves de criptografia para uso em diversos
serviços da AWS, geralmente para dados, arquivos no S3.<br>

#
## Pergunta 3: 
Você irá disponibilizar uma aplicação crítica e com dados sensíveis na Internet. Qual é o
serviço que te ajuda a identificar vulnerabilidades de segurança e riscos de exposição de
acordo com as melhores práticas e compliance?

- [X] O AWS Inspector
- [ ] O AWS Macie
- [ ] O AWS KMS
- [ ] O AWS GuardDuty

### Explicação

**Correta**

O Amazon Inspector é um serviço automatizado de gerenciamento de vulnerabilidade
que verifica continuamente as workloads da AWS em busca de vulnerabilidades de
software e exposição não intencional à rede.
https://aws.amazon.com/inspector/Qnc2=type_a

**Incorretas**

O Amazon GuardDuty é um serviço de detecção de ameaças que monitora
continuamente atividades mal-intencionadas e comportamentos não autorizados para
proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.<br>
O Amazon Macie é um serviço de rança e privacidade de dados totalmente
gerenciado que usa machine learning e correspondência de padrões para descobrir e
proteger seus dados confidenciais na AWS. À medida que as organizações gerenciam
volumes crescentes de dados, identificar e proteger seus dados confidenciais em escala
pode se tornar cada vez mais complexo, caro e demorado. O Amazon Macie automatiza a
descoberta de dados confidenciais em escala e reduz o custo da proteção de seus dados<br>
O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves
criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em
seus aplicativos https://aws.amazon.com/pt/kms/

#

## Pergunta 4: 

Sua empresa deseja otimizar o custo com a utilização do S3 e você notou que existem
muitas logs armazenadas e que poderiam ser deletadas após 30 dias da criação. O que
pode ser feito para essa otimização?

- [X] Configurar no S3 Lifecycle para que os objetos expirem em 30 dias para serem automaticamente excluídos.
- [ ] Criar uma cópia destes objetos em outra região
- [ ] Configurar o CloudWatch para monitorar o S3 e enviar um email SQLicitando a exclusão dos arquivos
- [ ] Criar uma cópia destes objetos em outra zona de disponibilidade

### Explicação
**Correta**

Configurar a expiração dos objetos para serem excluídos de forma automática quando
vencerem. https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html

**Incorretas**

As demais opções são formas de gerenciar e monitorar os objetos, não trazem redução
de custos
#

## Pergunta 5: 

Sua empresa iniciou um processo de transformação digital de todas as suas plataformas
e decidiu utilizar uma arquitetura de sistemas orientada a eventos. Qual dos serviços
abaixo pode ser utilizado como um barramento escalável de eventos para facilitar a
criação dessa arquitetura?

- [ ] Amazon EventSync
- [ ] Amazon Lambda
- [ ] Amazon SQS
- [X] Amazon EventBridge*

### Explicação
**Correta**

O EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação
de aplicações orientadas por eventos em escala usando eventos gerados com base em
suas aplicações, aplicações integradas de software como serviço (SaaS) e serviços da
AWS. Você pode configurar regras de roteamento para determinar para onde enviar seus
dados para criar arquiteturas de aplicações que reagem em tempo real às suas origens
de dados com o consumidor e editor de eventos completamente dissociados
https:Waws.amazon.com/pt/eventbridge/?nc2=h_ql_prod_ap_eb

**Incorretas**

O Lambda é utilzado para implementar funções sem servidores.<br>
O SOS - Simple Queue Service é utilizado para enfileirar mensagens e desacoplar o
serviços dos sistemas<br>
O Amazon EventSync não é um serviço existente na AWS

#
## Pergunta 6: 
Qual é a forma de permitir que seus serviços sejam expostos sempre no mesmo
endereço IP e de possibilitar que os hosts associados a ele sejam substituídos de forma
simples na sua infraestrutura?

- [X] Utilizando um IP Elástico*
- [ ] Utilizando um IPV6
- [ ] Utilizando um IPV4
- [ ] Utilizando o Route 53

### Explicação
O IP Elástico permite manter um IP ativo como porta de entrada e também que sejam
feitas associações de IPS dinâmicos a cada provisionamento de uma nova máquina, uma
vez que nesses cenários os IPV4 mudam. https:Waws.amazon.com/pt/ec2/features/

#

## Pergunta 7: 

Qual é o banco de dados relacional totalmente gerenciado pela AWS e que pode ser 5 x
mais rápido que o MySQL?

- [ ] ManaDb
- [ ] Neptune
- [ ] DynamoDb
- [X] Aurora

### Explicação

**Correta**

O Amazon Aurora é um banco de dados compativel com MySQL e PostgreSQL criado
para a nuvem e que combina a performance e a disponibilidade de bancos de dados
empresariais tradicionais com a simplicidade e a economia de bancos de dados de
código aberto.<br>
O Amazon Aurora é até cinco vezes mais rápido que bancos de dados MySQL padrão e
três vezes mais rápido que bancos de dados PostgreSQL padrão. O serviço oferece a
segurança, a e a confiabilidade de bancos de dados comerciais por um
décimo do custo. O Amazon Aurora é gerenciado pelo RDS, que automatiza tarefas
administrativas demoradas como provisionamento de hardware, configuração do banco
de dados, aplicação de patches e backups. https://aws_amazon.com/pt/rds/aurora/?nc2=type_a&aurora-whats-new_sort-
by—item .add itio nal Fields. postDateTime&au rora-whats-new.sort-order=desc

**Incorretas**

O Neptune é um banco de dados totalmente gerenciado pela AWS, noSQL e baseado em
Grafos.<br>
O DynamoDb é um banco de dados totalmente gerenciado pela AWS, noSQL„ baseado
em chave e valon<br>
O MariaDb é um banco de dados totalmente gerenciado pela AWS quando utilizado no
RDS e não gerenciado quando instalado instalado diretamente numa instância EC2, é
relacional, não é 5 x mais rápido que o mySQL.

*Nota*<br>
Os bancos de dados gerenciados são administrados pela AWS, diminuem a necessidade
da mão de obra de instação e manutenção para o cliente, enquanto banco de dados não
gerenciados ou gerenciados pelo cliente são bancos que precisam da atuação do cliente
na sua instalação e manutenção. 1.1m caso típico é a instalação de algum mecanismo de
banco de dados de mercado em uma instância do EC2. Os clientes que desejam um
maior controle na administração do banco de dados podem optar por essa segunda
opção

#

## Pergunta 8: 

Qual é a opção de armazenamento default do serviço S3?

- [ ] Glacier
- [ ] Infrequent Access
- [X] Standard*
- [ ] Frequent Access

### Explicação

**Correta**
O Standard está definido como padrão por oferecer diversas otimizações, usar as outras
opções sempre devem ser avaliadas de acordo com requisitos de qualidade da
aplicação, como tempo de resposta necessário, entre outros.
https:Waws.amazon.com/s3/storage-classes/?nc=sn&loc=3

**Incorretas**

As demais classes precisam ser configuradas e irão apresentar um tempo de resposta de
recuperação maior do que no modelo padrão.<br>
Uma classe não citada e que pode ajudar na movimentação entre as classes de forma
automática é a Inteligente Tiering.

#

## Pergunta 9: 
Qual é o serviço que garante que você tenha o correto número de instâncias EC2
disponíveis para lidar com a carga da sua aplicação?

- [ ] Route53
- [X] EC2 Auto Scaling
- [ ] VPC
- [ ] ELB

### Explicação

**Correta**

O Amazon EC2 Auto Scaling ajuda a manter a disponibilidade das aplicações e permite
adicionar ou remover instâncias do EC2 automaticamente de acordo com as condições
que você definir. É possível usar os recursos de gerenciamento de frota do EC2 Auto
Scaling para manter a integridade e a disponibilidade da sua frota Você também pode
usar os recursos de escalabilidade dinâmica e preditiva do EC2 Auto Scaling para
adicionar ou remover instâncias do EC2. A escalabilidade dinâmica responde às
mudanças na demanda e a escalabilidade preditiva agenda automaticamente o número
certo de instâncias do EC2 com base na demanda prevista
https://aws.amazoncom/pt/ec2/autoscaling/

**Incorretas**

O Amazon Route 53 é um web service DNS na nuvem altamente disponivel e escalável.
Ele foi projetado para oferecer aos desenvolvedores e empresas uma maneira altamente
confiável e econômica de direcionar os usuários finais aos aplicativos de Internet,
convertendo nomes como wwwexample.com para endereços IP numéricos como
192.0.2.1, usados pelos computadores para se conectarem entre si. O Amazon Route 53
também é totalmente compatível com o IPv6
https•Waws.amazon.com/pt/route53/Pnc2=type_a<br>
O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações
entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IR,
funções do Lambda e dispositivos virtuais. O serviço pode lidar com a carga variável de
tráfego das aplicações em uma única zona de disponibilidade ou em diversas zonas de
disponibilidade
https://aws.amazon.com/pt/elasticloadbalancing/?whats-new-cards-elb-sort-
bFitem .add itionalFields. postDateTime&whats- new-cards-elb. sort-order—desc<br>
O AWS VPC - Virtual Private Cloud permite que você crie uma rede privada iSQLada para
alocar diversos recursos.

#

## Pergunta 10: 
Você implantou uma aplicação em produção que não está funcionando e na log existe
uma mensagem de acesso negado ao DynamoDB. Qual serviço você precisa checar e
configurar corretamente para validar esse acesso?

- [x] O AWS IAM roles
- [ ] O AWS IAM Policy
- [ ] O AWS Config
- [ ] O AWS Cognito

### Explicação
**Correta**

(Correto)
Através de roles podemos gerenciar os acessos das aplicações aos serviços da AWS,
como o DynamoDB, RDS, entre outros.

**Incorretas**

AWS Config você gcde usar para gerenciar e monitorar as configurações dos seus
serviços<br>
IAM Policy são as políticas relacionadas a cada serviços e que podem ser adicionadas a
pessoas ou roles, com uma série de permissões ou restrições<br>
AWS Cognito é o serviço utilizado para fornecer autenticação para aplicações web e
mobile<br>

#

## Pergunta 11: 

Quais dos seguintes planos de suporte oferecem acesso ao atendimento ao cliente,
whitepapers, documentações e fóruns de suporte 24x7? (Selecione 2)

- [x] Basic
- [ ] Full
- [x] Enterprise
- [ ] Reserved

### Explicação

**Correta**

Todos os planos desde o Basic oferecem esses serviços. Basic, Developer, Business,
Entrerprise on ramp e Enterprise.<br>
Nas opções listadas só tem Basic e Enterprise e são as únicas possíveis pois as outras
não são planos de suporte existentes.<br>
Para os planos business e enterprise existe uma opção de suporte técnico aprimorado
24x7, que é mais exclusivo e que dá acesso aos engenheiros da AWS por telefone e e-
mail, mas que só seria a resposta caso a pergunta estivesse relacionada a suporte
técnico aprimorado.<br>
Maiores detalhes em: https://aws.amazon.com/premiumsupport/plans/

**Incorretas**
Full e Reserved não são nomes de plano de suporte na AWS.

#

## Pergunta 12: 
Você implementou um sistema com arquitetura de microsserviços e precisa depurar
cada um deles, partir desde a requisição do usuário para entender a performance e
identificar oportunidades de melhorias. Qual serviço da AWS é o mais indicado para essa
finalidade (tanto em ambiente de desenvolvimento quanto em ambiente de produção)?

- [ ] AWS CloudWatch
- [ ] AWS CloudSearch
- [ ] AWS OpenSearch
- [x] AWS X-Ray

### Explicação
**Correta**

O AWS X-Ray rastreia as SQLicitações do usuário enquanto percorrem todo o aplicativo.
Ele agrega os dados gerados por serviços e recursos individuais que compõem o
aplicativo, oferecendo uma visão completa do seu
desempenho.https://aws.amazon.com/pt/xray/?nc2=h_ql_prod_dt_xray

**Incorretas**

O AWS CloudSearch é um serviço que permite a implementação de um serviço de busca
dentro de uma aplicação.<br>
AWS ElasticSearch é um serviço para armazenar, analisar e correlacionar uma grande
quantidade de dados de logs de seus aplicativos para identificar e reSQLver gargalos de
desempenho e problemas de disponibilidade. OpenSearch é uma bifurcação do
ElasticSearch e Kibana de código aberto, licenciada sob a ALv2 e orientada pela
comunidade.
https://aws.amazon.com/pt/opensearch-service/the-elk-stack/what-is-ElasticSearch/<br>
O AWS CloudWatch é utilizado para gerar métricas e monitorar diversos serviços e
aplicativos na AWS.


#

## Pergunta 13: 
Seu time de desenvolvimento identificou que um banco de dados relacional está com
baixa performance, a concorrência entre um grande volume de consultas e outras ações
na base de dados têm aumentando a latência no tráfego dos dados. Qual é a maneira
mais ágil e econômica de reSQLver este problema?

- [ ] Atualizar a role de acesso ao banco
- [ ] Criar novas instâncias do RDS em outra zona de disponibilidade.
- [ ] Substituir o RDS pelo Dynamo
- [x] Fazer o uso de Read Replicas

### Explicação

**Correta**

Com o uso de Read Replicas você pode aumentar a escalabilidade e melhorar o tráfego
dos seus dados direcionando os processos somente de leitura para cópias das bases de
dados
https://aws.amazon.com/rds/features/

**Incorretas**

As roles de acesso a dados não tem nenhuma relação com performance, são serviços
que autorizam ou negam os acessos.<br>
A substituição do banco de dados de um banco de dados relacionais (RDS) pelo
DynamoDB não é algo comum, uma vez que são banco de dados para usos diferentes e
esse tipo de estratégia exigiria grandes alterações do backend da aplicação.<br>
Criar novas instâncias do RDS multi-AZ é para aumentar a disponibilidade e tolerância a
falhas e também não é a opção mais econômica para esse cenário.

#

## Pergunta 14: 
Sua empresa deseja lançar um novo produto e para isso precisa criar um novo domínio
público para associá-lo a um novo site. Qual é a maneira mais rápida de fazer isso?

- [x] Criar um novo domínio no AWS Route53
- [ ] Desenvolver o novo site no AWS BeanStalk, que provisiona toda a infra para o desenvolvedor apenas programar.
- [ ] Criar um servidor de domínio numa instância AWS EC2 e incluir o novo domínio
- [ ] Criar um novo domínio no RegistroCom

### Explicação
**Correta**

AWS Route53

**Incorretas**

Com RegistroCom, além do registro será necessário configurar o Route53<br>
O EC2 não deve ser utilizado como servidor DNS público<br>
O Elastic BeanStalk provisiona a infra para o desenvolvedor implantar a aplicação, mas
isso não inclui o registro de domínios.

#

## Pergunta 15: 
Sua empresa deseja padronizar e versionar as configurações para a criação de todos os
bancos de dados, além disso, deseja que esses serviços sejam implementados e
atualizados em toda os servidores de forma automatizada, utilizando pipelines de CI/CD.
Qual é o serviço recomendado para esse requisito?

- [ ] AWS CodePipeline
- [ ] AWS IAC
- [ ] AWS RDS
- [x] AWS CloudFormation

### Explicação

**Correta**

AWS CloudFormation<br>
Arquivos Contendo o IAC, Infraestrutura como código, podem ser versionados e
atualizados de forma automatizada com o uso de CloudFormation
https://aws.amazon.com/pt/cloudformation/

**Incorretas**

AWS CodePipeline é utilizado para montar uma esteira de CI/CD para desenvolvimento
de aplicações<br>
IAC é uma sigla utilizada para definir Infraestrutura como serviço, que é o que o
CloudFormation entrega, porém um serviço com o nome AWS IAC não existe.<br>
AWS RDS é o serviço utilizado para Gerenciar Bancos de Dados com diversas
funcionalidades, entretanto não oferece o serviço necessário no cenário citado na
questão.

#

## Pergunta 16: 
Você precisa implementar uma estratégia de DR (Recuperação de Desastre) na sua
empresa, qual é a recomendação de melhor uso do AWS RDS?

- [ ] Multi A-Z (Distribuir em zonas de disponibilidade diferentes)
- [ ] Multi Regions (Distribuir em regiões diferentes)
- [ ] Implementar uma cópia do banco numa instância EC2
- [x] Read Replicas (Fazer cópias de leitura)

### Explicação
**Correta**

Estratégia Multi Region<br>
https://aws.amazon.com/rds/features/read-replicas/<br>
No link tem uma tabela comparando as 3 estratégias de implantações, Multi-AZ, Multi-Regiões e Read Replicas.

**Incorretas**

Multi-AZ é para aumentar a disponibilidade<br>
Muti-Regiões para DR e Read Replicas para escalabilidade.<br>

#

## Pergunta 17: 

Você deseja monitorar o percentual de memória que os seus servidores estão utilizando
em determinando período do dia. Qual serviço da AWS pode ser utilizado para essa
finalidade?

- [ ] AWS DataSync
- [x] AWS CloudWatch
- [ ] AWS Cost Explorer
- [ ] AWS CloudTrail

### Explicação
**Correta**

Com o AWS CloudWatch você pode monitorar os recursos da sua infraestrutura

**Incorretas**

O CloudTrail pode ser utilizado para realizar logs de eventos relacionados a api de
serviços.<br>
O Cost Explorer é para acompanhar os gastos da sua infraestrutura.<br>
O DataSync realiza a transferência de dados de forma automatizada entre ambientes on
premise e AWS.<br>

#

## Pergunta 18: 
Você está desenvolvendo uma aplicação mobile e precisa implementar o
armazenamento e sincronismo de dados para vários dispositivos. Qual é o serviço AWS
que pode ser utilizado para esse fim?

- [X] AWS Cognito
- [ ] AWS ElastiCache
- [ ] AWS DynamoDB
- [ ] AWS Redis

### Explicação
**Correta**

Além de fornecer um serviço de autenticação robusto para aplicativos móveis, o Amazon
Cognito permite o salvamento de dados num banco local de chave-valor para depois
realizar o sincronismo.
https://aws.amazon.com/pt/cognito/getting-started/

**Incorretas**

O ElastiCache permite o armazenamento em memória para ser utilizados por aplicações
escaláveis para guardar informações de sessão, consultas de bancos de dados, entre
outros.<br>
O Redis é ofertado pelo ElastiCache para prover cache de para as aplicações.<br>
O DynamoDb é o banco de dados totalmente gerenciado pela AWS, NoSql de
chave/valor<br>

#

## Pergunta 19: 
Você lidera um pequeno time desenvolvimento e deseja utilizar uma arquitetura de
microsserviços com conteiners. Qual serviço pode auxiliá-lo numa abordagem sem
servidor e que traz velocidade nas entregas, uma vez que você não precisa se preocupar
com questões de infraestrutura?

- [ ] ECR
- [ ] Ecs
- [ ] EKS
- [X] Fargate

### Explicação

**Correta**

O Fargate adiciona a possibilidade de execução de contaiiner sem servidor ao ECS,
diminuindo a mão de obra relacionada a configuração de ambiente.
https://aws.amazon.com/fargate/?nc2=h_ql_prod_ct_far&whats-new-cards.sort-
by=item.additionaIFieIds.postDateTime&whats-new-cards.sort-order=desc&fargate-
blogs.sort-by=item.additional

**Incorretas**

O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado
de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente
aplicações conteinerizadas.<br>
O Amazon Elastic Kubernetes Service (Amazon EKS) executa o plano de controle e
orquestração de containers com Kubernetes em várias zonas de disponibilidade, detecta
automaticamente e substitui nós do plano de controle com problemas de integridade e
oferece atualizações e aplicação de patches sob demanda e sem tempo de inatividade.<br>
O Amazon Elastic Container Registry (Amazon ECR) é um registro de contêiner
totalmente gerenciado que facilita o armazenamento, o gerenciamento, o
compartilhamento e a implantação de imagens e artefatos de contêiner em qualquer
lugar

#

## Pergunta 20: 

Uma das formas de garantir a elasticidade e economia no uso do EC2 é mantendo os
arquivos de programas e de sistemas em recursos computacionais distintos. Qual
serviço pode ser utilizado para isso?

- [ ] S3
- [ ] O Git
- [ ] CodeCommit
- [X] O EBS

### Explicação
**Correta**

Numa implementação padrão do serviço EC2 é necessário definir o tipo de máquina que
irá processar as instruções, e o tipo de EBS para armazenar e persistir os dados. Isso
permite que o EC2 seja ligado e desligado de acordo com o uso e que os dados fiquem
salvos no EBS durante esses processos.
https:Waws.amazon.com/pt/ec2/faqs/

**Incorretas**

O Git é um aplicativo para fazer o gerenciamento e gestão de código fonte.<br>
O CodeCommit é utilizado para gerenciar código fonte no modelo Git, semelhante ao
GitHub, GiTIab, etc.<br>
O S3 é utilizado para armazenar arquivos em forma de objeto (documento + metadado
do documento) em estruturas de Buckets.<br>

#

## Pergunta 21: 
Você precisa implementar no seu site uma funcionalidade para realizar pesquisas em
todas as páginas e arquivos para facilitar a navegação e experiência do seus usuário.
Qual SAAS disponível na AWS fornece ferramentas robustas para cumprir essa finalidade
e que pode ser facilmente utilizada na sua aplicação?

- [ ]Amazon CloudWatch
- [ ]Amazon Athena
- [X]*Amazon CloudSearch*
- [ ]Amazon OpenSearch

### Explicação
**Correta**

Amazon CloudSearch
https://aws.amazon.com/pt/cloudsearch/?nc2=h_ql_prod_an_cs

**Incorretas**

O Athena é um serviço servless que permite a realização de consultas utilizando SQL em
Buckets do S3.<br>
O OpenSearch é um conjunto distribuído, orientado à comunidade, com licença Apache
2.0 de pesquisa e análise de código 100% aberto usado para uma ampla variedade de
casos de uso, como monitoramento de aplicações em tempo real, análise de logs e
pesquisa de sites.<br>
O CloudWatch permite oferece a geração de métricas e monitoramento para diversos
serviços e aplicações da AWS.

# 
## Pergunta 22: 
Qual é a melhor descrição para o conceito de tolerância a falha?

- [ ]A habilidade de um sistema crescer e provisionar novos recursos para continuar executando suas cargas de trabalho sem interrupção
- [ ]A habilidade de um sistema nunca falhar
- [X]A habilidade de um sistema permanecer em funcionamento mesmo se um dos seus componentes falhar.
- [ ]A habilidade de um sistema exibir mensagens de falhas para os usuários.

### Explicação
**Correta**

Uma das premissas do desenvolvimento de aplicações resilientes é saber que os
componentes podem falhar e ter um plano para que eles continuem funcionando mesmo
assim permanecendo confiáveis e resilientes. Na AWS essa premissa está no pilar de
confiabilidade do Well-Architect Framework, que ajuda arquitetos de nuvem a
construirem infraestruturas seguras, resilientes, eficientes e de alta performance para
aplicações e cargas de trabalho. Baseado em 6 pilares (excelência operacional,
segurança, confiabilidade, eficiência de performance, otimização de custos,
sustentabilidade), o AWS Well-Architected Framework fornece uma abordagem
consistente para que clientes e parceiros avaliem arquiteturas e implementem designs
que podem se expandir com o tempo com economia e qualidade.
https://aws.amazon.com/pt/architecture/well-architected/?nc2=h_ql_le_wa&wa-lens-
whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-
order=desc

**Incorretas**

Nenhum serviço possui a habilidade de nunca falhar. Todo componente pode falhar em
hardwares, softwares, infraestrutura, redes e etc. Numa visão de tolerância a falhas não
pode-se contar com isso.<br>
A habilidade do sistema provisionar mais recursos sob demanda (on demand) para
atender as cargas de trabalho adequadas é conhecida como escalabilidade.<br>
A exibição de mensagens de erro podem ser requisitos de neçõcio ou requisitos de
qualidade e não tolerância a falhas. Junto com as logs dos componentes é conhecida
como observabilidade.

#

## Pergunta 23: 
Qual dos seguintes serviços de bancos de dados é totalmente gerenciado pela AWS?

- [ ] SQL Server
- [ ] MySql
- [ ] MariaDB
- [X] DynamoDB

### Explicação
**Correta**

O Amazon DynamoDB é um banco de dados de chave-valor NoSQL, sem servidor e
totalmente gerenciado, projetado para executar aplicações de alta performance em
qualquer escala.<br>
Quando um serviço é totalmente gerenciado o cliente não precisa se preocupar com
nada que está relacionado a sua implementação, como instalação, atualizações da
infraestrutura. A AWS faz todo o gerenciamento e o cliente utiliza apenas as APIS destes
serviços para a criação das tabelas, gravação e recuperação dos dados.<br>
No caso do
Dynamo, o cliente faz o uso do conSQLe ou das APIS para realizar a maior parte das
tarefas, sem se preocupar com a instalação do banco.
https://aws.amazon.com/pt/dynamodb/?nc2=type_a

**Incorretas**
As demais opções são sistemas gerenciadores de bancos de dados que podem ser
utilizados juntos com o RDS e totalmente gerenciados pela AWS ou instalados no EC2 e
gerenciado pelo cliente.<br>
Como as demais opções não falaram do RDS, não é possível afirmar se é gerenciado pela
AWS ou pelo cliente, desta forma, a opção correta é o DynamoDB.<br>
Quando o cliente deseja gerenciar o banco, ele fica responsável por todo o processo de
instalação, atualizações, melhorias de performance, etc. Configura um modelo uso laaS
pois só está utilizando o servidor como infraestrutura.

#

## Pergunta 24: 
Qual é o serviço utilizado para provisionar Desktops utilizando Windows ou Linux?

- [ ] EC2
- [X] Amazon WorkSpaces
- [ ] Amazon Desktops
- [ ] Amazon CLI

### Explicação
**Correta**

Com o Amazon Workspaces é possível provisionar um grande número de máquinas
virtuais para uso como desktops.
https://aws.amazon.com/workspaces/?nc2=h_ql_prod_eu_wspa&workspaces-
blogs.sort-by=item.additionalFields.created

**Incorretas**
O EC2 - Elastic Compute Cloud - fornece instâncias de servidores com diversas
configurações e opções de processamento, memória e rede<br>
O Amazon CLI - Command Line Interface é uma interface por linha de comando que
você pode instalar pra fazer uso no seu desktop<br>
O Amazon Desktops não existe

#

## Pergunta 25: 

Quais são os cinco planos de suporte ofertados pela AWS?

- [ ] Basic, Developer, Business, Advanced, Enterprise On-Ramp
- [ ] Standard, Developer, Business, Enterprise, Enterprise On-Ramp
- [ ] Bronze, Silver, Gold, Diamond, Ruby
- [X] Basic, Developer, Business, Enterprise On-Ramp, Enterprise

### Explicação

**Correta**

Basic, Developer, Business, Enterprise On-Ramp e Enterprise.
E importante conhecê-los e explorar as características que os diferenciam também.
Cada um oferece um pacote de serviços e recomendações de acordo com o objetivo do
uso da AWS.<br>
Recomendo a leitura desta página que mostra todo os detalhes:
https://aws.amazon.com/pt/premiumsupport/plans/

Nota: Publicado: Nov 24, 2021<br>
A Amazon Web Services (AWS) anunciou a disponibilidade geral do Enterprise On-Ramp,
um novo nível de suporte entre os atuais Business e Enterprise para ajudar os clientes
que estão começando sua jornada na nuvem e precisam de orientação especializada
para crescer e otimizar na nuvem<br>
https:Waws.amazon.com/pt/about-aws/whats-new/2021/11/enterprise-on-ramp-
general-availability/

**Incorretas**

Standard, Advanced, Bronze, Silver, Gold, Diamond, Ruby não existem na AWS.

#

## Pergunta 26: 

Baseado nos pilares de excelência operacional, segurança, confiança, performance
eficiente, sustentabilidade e otimização de custos, qual é o Framework que ajuda os
arquitetos cloud a construirem aplicações seguras, com alta performance, resilientes e
eficientes?

- [ ] AWS Pillar
- [ ] AWS CloudFormation
- [X] AWS Well-Architected
- [ ] Framework .Net

### Explicação
**Correta**

AWS Well-Architected é composto pelos 6 pilares citados na questão.
https://wa.aws.amazon.com/wat.pillars.wa-pillars.pt_BR.html

**Incorretas**

O AWS CloudFormation oferece uma forma fácil de modelar uma coleção de recursos
relacionados da AWS e de terceiros, provisioná-la com rapidez e consistência e gerenciar
todo o seu ciclo de vida mediante o tratamento da infraestrutura como código<br>
O Framework.net e o AWS Pillar não são serviços da AWS.

#
## Pergunta 27: 
Qual opção descreve a função do serviço Elastic Load Balancer?

- [ ] Instanciar uma nova máquina quando uma das máquinas apresenta falha
- [ ] Criar um cluster de máquinas dentro da mesma zona de disponibilidade
- [ ] Distribuir o tráfego de entrada entre instâncias em diferentes regiões
- [X] Distribuir o tráfego de entrada entre suas instâncias

### Explicação
**Correta**

(Correto)
Distribuir o tráfego entre instâncias na mesma região, geralmente alocadas em mais de
uma zona de disponibilidade.
https://aws.amazon.com/search/?searchQuery=eIb

**Incorretas**
O ELB não é o responsável por instâncias uma nova máquina quando uma apresenta
falha, ele é o serviço que deixa de direcionar o tráfego para essa máquina e balanceia a
carga só entre as máquinas saudáveis e disponíveis.<br>
Para o balanceamento de carga entre regiões, o mais adequado é usar alguma estratégia
do Route53, como geolocalização, Volume de tráfego, etc.<br>
O ELB é utilizado para balancear as cargas em mais de uma zona de disponibilidade e
também não cria um cluster de máquinas, apenas direciona as cargas entre elas.

#

## Pergunta 28: 

Utilizando os serviços da AWS, qual é a sequência esperada numa pipeline de CI/CD?

- [X] CodeCommit, CodeBuild, CodeDeploy
- [ ] CodeCommit, CodeDeploy, CodeBuild
- [ ] CodeBuild, CodeCommit, CodeDepIoy
- [ ] CodeBuiId, CodeDepIoy, CodeCommit

### Explicação
**Correta**

Essa é uma sequência lógica numa esteira de desenvolvimento:
CodeCommit - Gerenciamento dos fontes através de funções do Git.
CodeBuild - Compilação e Testes automatizados.
CodeDeploy - Implantação.

**Incorretas**

As demais ordens não apresentam a sequência lógica da esteira.

*Nota*<br>
Os serviços apresentados são orquestrados através do serviço CodePipeline, que é a
esteira que integra todos os serviços mencionados na questão.
https://aws.amazon.com/pt/codepipeline/<br>

Em questões sobre ciclos de desenvolvimento também é possível encontrar a citação do
CodeStar, que é um serviço que permite o gerenciamento dos recursos do projeto,
pessoas, permissões e recursos de infraestrutura, CodePipeline e os demais.<br>
O CodeStar também oferece modelos de projetos, que diminuem a necessidade de diversas
configurações e trazem muita agilidade para todo o processo de desenvolvimento de
uma aplicação.
https://docs.aws.amazon.com/pt_br/codestar/latest/userguide/welcome.html

#

## Pergunta 29: 

Numa migração de sistemas, você percebeu que existem dados na sua aplicação que
raramente são usados e que poderiam ser mantidos em arquivos somente para fins de
auditoria. Qual é o serviço da AWS que pode ser utilizado para esse objetivo com o
menor custo possível?

- [ ] S3 Standard
- [X] S3 Glacier
- [ ] S3 Infrequent Access
- [ ] S3 Intelligent Tiering

### Explicação
**Correta**

O Serviço S3 Glacier permite fazer a guarda destes dados de uma forma mais
econômica, porém com um tempo de recuperação mais lento.
https://aws.amazon.com/pt/glacier/faqs/

**Incorretas**

O S3 Standard oferece um armazenamento de objetos com altos níveis de resiliência,
disponibilidade e performance para dados acessados com frequência. O custo é maior
que o Glacier.<br>
S3 Intelligent Tiering é a única classe de armazenamento em nuvem que oferece
economia automática de custos de armazenamento quando os padrões de acesso a
dados mudam, sem impacto na performance ou sobrecarga operacional. O custo é maior
que o Glacier.<br>
O S3 Standard-IA é indicado para dados acessados com menos frequência, mas que
exigem acesso rápido quando necessários. O custo é maior que o Glacier.

#

## Pergunta 30: 
Você trabalha numa agência de publicidade que deseja implantar um site com o
conteúdo estático para fazer a primeira divulgação de um produto. Qual é o serviço da
AWS mais indicado para esse cenário?

- [ ] EC2
- [ ] Docker
- [X] S3
- [ ] EFS

### Explicação
**Correta**

O S3 permite o armazenamento de objetos como arquivos hTIm, js, cs eliminando a
necessidade de uso do EC2 trazendo muito mais economia, disponibilidade e resiliência
para as suas SQLuções.

**Incorretas**

O EFS - Elastic File System é um serviço utilizado para implementar um serviço de
arquivos na sua arquitetura associado a instâncias EC2. Apesar de servir para armazenar
arquivos estáticos não é o mais fácil e barato de implementar.<br>
O EC2 - Elastic Computing Cloud oferece diversas configurações de máquinas para
computação, associado a um EBS ou EFS poderia manter páginas web, entretanto não é
a forma mais barata e ágil.<br>
O Docker é utilizado para microserviços e sua implementação na AWS é possível através
do ECS - Elastic Container Service.

#

## Pergunta 31: 
Qual afirmação abaixo não se refere ao AWS Lambda?

- [X] Permite o gerenciamento total dos recursos de infraestrutura
- [ ] Processa dados sem servidor
- [ ] Pode ser acionado diretamente pelo AWS S3
- [ ] Pode ser acionado diretamente pelo AWS SNS

### Explicação
**Correta**

Lambda é totalmente gerenciado pela AWS e faz o provisionamento automático para
executar as funções.<br>
E importante ter atenção com questões que tem uma negação (não) no início pois
podem inverter as respostas que parecem óbvias.
https://aws.amazon.com/pt/lambda/?nc2=h_ql_prod_serv_lbd


#

## Pergunta 32: 
Qual é o usuário utilizado para acessar o AWS ConSQLe pela primeira vez e que possui
acesso a todos os recursos da conta? (não sendo recomendado para uso no dia a dia.)

- [ ] AWS IAM
- [ ] AWS full user
- [X] AWS account root user
- [ ] AWS Administrator

### Explicação
**Correta**

O root user é informado no primeiro acesso da sua conta e só é recomendado para as
primeiras configurações dos demais acessos, uma vez que ele possui acessos ilimitados
a todos os serviços da conta.<br>
https:Wdocs.aws.amazon.com/lAM/latest/UserGuide/introduction.html

**Incorretas**

Full User e Administrador não são conceitos utilizados nestes acessos.<br>
O AWS IAM é o serviço utilizado para gerenciar os usuários, roles e serviços, não é o
usuário em si.

# 

## Pergunta 33: 
Sua aplicação fornece dados através de APIS REST para diversas aplicações diferentes.
Pensando num cenário de futuras manutenções e evoluções dos seus serviços, qual
opção abaixo pode melhor auxiliar a sua arquitetura a manter várias versões da mesma
API sendo executadas simultaneamente e não exigir que todos os consumidores
realizem adequações nas chamadas ao seu serviço?

- [ ] AWS Zuul
- [ ] AWS Route53
- [ ] AWS EventBridge
- [X] API Gateway

### Explicação
**Correta**

O API Gateway permite esse tipo de convivência
https://aws.amazon.com/pt/api-gateway/features/

**Incorretas**

O AWS Zuul não existe<br>
O AWS EventBridge é um barramento de eventos sem servidor que torna mais fácil a
criação de aplicações orientadas por eventos em escala usando eventos gerados com
base em suas aplicações, aplicações integradas de software como serviço (SaaS) e
serviços da AWS.<br>
O AWS Route53 é um web service Domain Name Server(DNS) na nuvem altamente
disponível e escalável

#

## Pergunta 34: 
O que é o MFA - Multi-Factor-Authentication (Autenticação Multi Fator)?

- [ ] Um serviço que permite a conexão entre a máquina do cliente e um servidor na AWS através de um arquivo contendo key pairs (par de chaves)
- [X] Um serviço que inclui uma etapa a mais no processo de autenticação de acesso a conta da AWS através do ConSQLe Web
- [ ] Um serviço para permitir que instâncias EC2 acessem banco de dados DynamoDb
- [ ] Um serviço que utiliza key pairs (par de chaves) na autenticação do usuário através da CLI (Linha de Comando)

### Explicação
**Correta**

Um serviço que inclui uma etapa a mais no processo de autenticação de acesso a conta
da AWS através do ConSQLe Web.<br>
Autenticação Multi Fator deve ser habilitada com algum
dispositivo de terceiros para a proteção do acesso via conSQLe. Um exemplo é o Google
Authenticator, que gera um código numérico a cada minutos que deve ser utilizado no
login.
https://docs.aws.amazon.com/pt_br/lAM/latest/UserGuide/id_credentials_mfa.html

**Incorretas**

Um serviço para permitir que instâncias EC2 acessem banco de dados DynamoDb são
roles (funções) definidas no IAM.<br>
Um serviço que permite a conexão entre a máquina do cliente e um servidor na AWS
através de um arquivo contendo key pairs (par de chaves) é uma conexão SSH.<br>
Um serviço que utiliza key pairs (par de chaves) na autenticação do usuário através da
CLI (Linha de Comando) é um processo de autenticação entre o cliente e AWS digitando
tais informações na linha de comando.<br>

*Nota*<br>
Além do processo de login, o MFA pode ser utilizado em outros processos, como:
- Deleção de bucktes do S3
- Login pelo Cognito para usuários finais em aplicações web e mobile

#

## Pergunta 35: 
Analise os serviços abaixo:

- *O primeiro serviço permite que aplicativos enviem mensagens críticas, em termos de
tempo, para vários assinantes através de um mecanismo de "push", eliminando a
necessidade de verificar periodicamente ou pesquisar por atualizações.*

- *O segundo é um serviço de fila de mensagens, usado por aplicativos distribuidos para
trocar mensagens através de um modelo de sondagem e pode ser usado para
desacoplar componentes de envio e recebimento.
Qual é a sequência abaixo que informa corretamente os dois serviços?*

- [ ] SQS e SNS
- [ ] SES e SNS
- [X] SNS e SQS
- [ ] SES e SQS

### Explicação
**Correta**

SNS - Simple Notification Service<br>
O Amazon Simple Notification Service (Amazon SNS) é um serviço de mensagens
totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de
aplicação para pessoa (A2P).<br>
https://aws.amazon.com/pt/sns/?whats-new-cards.sort-
by—item ditio nal Fields. postDateTime&whats- new-cards.so rt-orde r=desc<br>

SQS - Simple Queue Service<br>
O Amazon Simple queue Service (Amazon SOS) oferece uma fila hospedada segura,
durável e disponível que permite integrar e desacoplar sistemas de software e
componentes distribuídos
https://docs.aws.amazoncom/pt_br/AWSSimplequeueService/latest/SOSDeveloperGui
de/welcome. html

**Incorretas**

As demais opções estão incorretas<br>
O SES - Simple Email Service é utilizado para fazer envio de emails.

# 

## Pergunta 36: 
Qual é a quantidade de dados que pode-se armazenar no S3?

- [ ] 5 Gigabytes
- [ ] 50 Gigabytes
- [X] A capacidade é virtualmente ilimitada
- [ ] 1 Terabyte

### Explicação
**Correta**

A medida que aumenta a necessidade de armazenamento, a AWS vai fornecendo mais
recursos para o S3, vai escalando totalmente gerenciado pela AWS com capacidade
virtualmente ilimitada.
https://aws.amazon.com/pt/s3/

**Incorretas**

Uma vez que a capacidade é virtualmente ilimitada, as demais opções limitam a
capacidade de armazenamento e estão erradas.<br>

*Nota*<br>
Um objeto do S3 possui o limite de até 5TB e é importante distingui-lo da capacidade do
S3 que pode armazenar vãrios objetos.

# 

## Pergunta 37: 

Qual opção que melhor descreve o modelo de Responsabilidade Compartilhada da AWS
(shared responsability)?

- [ ] O desenvolvedor é responsável por implantar a aplicagão, enquanto o gestorfaz a aprovação
- [ ] A AWS protege o data center, enquanto a Microsoft protege o windows
- [X] A AWS protege o data center, enquanto o cliente protege as aplicações.
- [ ] O cliente protege as aplicaqóes, enquanto usuário protege sua senha

### Explicação
**Correta**

A AWS protege o data center, enquanto o cliente protege as aplicaqóes.
O modelo de responsabilidade compartilhada explora bastante quais são as diferentes
atividades de responsabilidade da AWS e do cliente dono de uma conta, para o melhor
uso de Cloud.<br>

No geral a AWS é responsável por tudo relacionado a infraestrutura dos datacenters e
redes (incluindo softwares do Hypervisor) e os clientes são responsãveis pela segurança
dos seus sistemas e aplicaqóes.<br>

A AWS protege o data center, faz manutenção em hardware, criptografa os dados na
camada fisica, atualiza softwares de base, mas se o cliente não desenhar uma aplicação
segura, deixar senhas expostas em git, não fizer as próprias criptografias, uso de
certificados e etc, isso é responsabilidade dele e não da AWS.<br>

**Incorretas**

As outras respostas não correlacionam a AWS com o cliente dono da conta, que são as
entidades mencionadas no modelo de responsabilidade compartilhada.

#

## Pergunta 38: 
Sua empresa tem um sistema que suporta em média 2000 usuários por dia, em dias com
o au mento de vendas, o sistema chega a 3000 usuários apresentando lentidão e
indisponibilidade. Como vocé automatizaria o processo para provisiona
automaticamente instáncias de servidor adicionais para suportar essas cargas em
periodos de pico?

- [X] Usando o Auto Scalling
- [ ] Incluindo mais uma máquina fisica e alterando o ELB
- [ ] Migrando a aplicaqáo para uma máquina melhor
- [ ] Implementando EBS Snapshots

### Explicação
**Correta**

Usando o Auto Scalling vocé pode configurar qual é a melhor estratégia para escalar sua
aplicação, incluindo e retirando máquinas, de acordo com a demanda de recursos,
aumentando a disponibilidade e reduzindo custos.<br>
O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade
para manter um desempenho constante e previsivel pelo menor custo possivel.<br>
Com o AWS Auto Scaling, é fácil configurar a escalabilidade de aplicativos para vários recursos
em diversos servigos.
https://aws.amazon.com/pt/autoscaling/

**Incorretas**

Incluir máquina fisica é algo incomum na cloud, uma vez que as instáncias, em sua
grande maioria, são virtualizadas. Existe até um modelo chamado de dedicated hosts,
mas que o uso por si Sd, não garante a esca•abilidade sem o uso do Auto Scalling
A implementagão do ELB garante o balanceamento das cargas entre as instáncias,
entretanto não é ele que inclui e retirar máquinas de acordo com a demanda. É uma pega
adicional para essa arquitetura para direcionar o tráfego assim que a máquina for
provisjonada pelo Auto Scalling Group.<br>
Migrar para uma máquina melhor melhoraria o desempenho da aplicagão, entretanto não
aconteceria de forma automática de acordo com a demanda de carga, não seria
escalável e nem a opção mais económica quando a carga diminuisse.
O EBS Snapshot é uma fotografia do block storage que pode ser usado para diversas
finalidades, porém para o processo de Auto Scalling, o ideal é usar uma imagem através
do AMI.

#

## Pergunta 39:
Quais recursos referem-se ao Amazon S3 (Selecione 2 alternativas)

- [ ] Elastic Load Balancer são balanceadores de carga
- [ ] Lambdas são funções sem servidores
- [X] Bucket é um conteiner de objetos
- [X] Objeto é um arquivo ou meta dado que descreve o arquivo

### Explicação
**Correta**

Amazon S3 é o serviço de armazenamento principal da AWS, é composto por Buckets,
que são criados para organizar objetos compostos por arquivos e metadados dos
arquivos.

**Incorretas**

Lambdas são funqóes sem servidores que não fazem parte do S3, está relacionada a
computação e não a armazenamento.<br>
ELB são balanceadores de carga entre instãncias que fazem parte do EC2.
https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html


#

## Pergunta 40: 
Recentemente vocé implementou uma aplicação piloto na sua empresa. Para realizar o
rollout do projeto, sua CTO pediu para vocé apresentar os gastos com infraestrutura
AWS durante o periodo para avaliação e aprovat;ão da expansão. Qual é o serviço que
fornece essas informaqóes?

- [X] AWS CostExplorer
- [ ] AWS Trusted Advisor
- [ ] AWS Inspector
- [ ] AWS Budgets

### Explicação
**Correta**

Com o AWS Cost Explorer vocé pode consultar os custos da sua infraestrutura a todo
momento.<br>
O AWS Cost Explorer tem uma interface fãcil de usar que permite visualizar, entender e
gerenciar os custos e o uso da AWS ao longo do tempo.<br>
Comece a usar rapidamente criando relatórios personalizados que analisam dados de
custos e uso, Analise dados de forma resumida (por exempla, custos e uso totais em
todas as contas) ou detalhe os dados de custos e uso para identificar tendéncias,
determinar causadores de custos e detectar anomalias.
https://aws.amazon.com/pt/aws-cost-management/aws-cost-explorer/

**Incorretas**

O AWS Trusted Advisor faz recomendaqóes que ajudam vocé a seguir as melhores
práticas da AWS. O Trusted Advisor avalia a sua conta através de verificações.<br>
O Amazon Inspector é um serviço de avaliação de segurança automático que ajuda a
melhorar a segurança e a conformidade dos aplicativos implantados na AWS. O Amazon
Inspector avalia automaticamente aplicativos em busca de exposiqóes, vulnerabilidades
ou discrepáncias em relação as melhores práticas<br>
O AWS Budgets é o serviço utilizado para definir orqamentos desejáveis para a uso e
incluir alertas para notificação de alertas sobre uso acima do esperado.

#

## Pergunta 42: 
Uma aplicação de terceiros irá gerar um arquivo num layout diferente do que o seu
sistema espera Qual é serviço da AWS que pode ser utilizado para transformar o arquivo
e carregã-lo no seu sistema?

- [ ] AWS DataSync
- [ ] AWS DMS
- [ ] AWS DTS
- [X] AWS Glue

### Explicação
**Correta**

Glue - E um serviço indicado para ETI - Extrair, transformar e carregar dados

**Incorretas**

O AWS DTS não é um serviço disponivel na AWS<br>
O AWS DataSync é utilizado para realizar a sincronização automatica entre dados da
infraestrutura on premise e da AWS.<br>
O DMS - Database Migration Service é o servico utilizado para realizar a migração de
banco de dados na AWS.

# 

## Pergunta 44: 
Qual é o serviço que vocé precisa configurar para controlar o tráfego de dados de
entrada e saida em um parque de servidores de bancos de dados, dentro da sua rede
privada na AWS?

- [X] AWS Security Group?
- [ ] AWS Shield
- [ ] AWS WAF
- [ ] AWS GuardDuty

### Explicação
**Correta**

AWS Securiiy Group é um serviG0 que permite agrupar vários servidores e implementar
regras para a entrada e saida de dados.<br>

**Incorretas**

O GuadDuty é um serviço de detecção de ameaqas que monitora continuamente
atividades mal-intencionadas e comportamentos não autorizados para proteger suas
contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.<br>
O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço
distribuida) que protege os aplicativos executados na AWS.<br>
O AWS WAF é um firewall de aplicaqóes Web que ajuda a proteger suas aplicaqóes Web
ou APIs contra bots e exploits comuns na Web que podem afetar a disponibilidade,
comprometer a seguranga ou consumir recursos em excesso.
https://aws.amazon.com/pt/


#

## Pergunta 45: 
O que é possivel fazer com o Amazon OuickSight?

- [ ] Capturar dados de diversos dispositivos através e streaming de dados de forma rápida
- [ ] Executar Map reduce em dados distribuidos
- [X] Criar DashBoards de Bl com uso de Aprendizado de Máquina (Machine Learning)
- [ ] Realizar consultas em objetos armazenados no S3

### Explicação
**Correta**

O Amazon OuickSight permite que todos em sua organização entendam seus dados por
meio de perguntas em linguagem natural, do uso de painéis interativos ou procurando
automaticamente padróes e discrepãncias com tecnologia de machine learning.
https://aws.amazon.com/pt/quicksight/

**Incorretas**

Capturar dados por streaming é o com o Kinesis<br>
Consultar no S3 é com o Athena<br>
Fazer MapReduce é com o EMR

#

## Pergunta 46: 

Numa estratégia de utilização de nuvem hibrida, onde vocé deseja manter seu workload
on-premises e parte dos arquivos na AWS. Qual opção abaixo oferece uma gama de
serviços para realizar essa finalidade de integração e armazenamento para sua
arquitetura?

- [ ] AWS Organizations
- [ ] AWS Database Migration Service
- [ ] Amazon Virtual Private Cloud (VPC)
- [X] AWS Storage Gateway
### Explicação
**Correta**

O AWS Storage Gateway é um conjunto de serviços de nuvem hibrida que oferece
acesso on-premises a armazenamento na nuvem praticamente ilimitado. Os clientes
usam o Storage Gateway para integrar o armazenamento da Nuvem AWS com workloads
Iocais para que possam simplificar o gerenciamento do armazenamento e reduzir os
custos de casos de uso de armazenamento fundamentais na nuvem hibrida

**Incorretas**

O AWS Database Migration Service (AWS DMS) ajuda vocé a migrar bancos de dados
para a AWS de modo rápido e seguro.<br>
O AWS Organizations ajuda vocé a gerenciar e controlar seu ambiente de maneira
centralizada medida que os neçõcios e seus recursos da AWS expandem. Usando o
AWS Organizations, vocé pode criar novas contas da AWS e alocar recursos, agrupar
contas para organizar seus fluxos de trabalho, aplicar politicas a contas ou grupos para
governança e simplificar o faturamento usando um ünico método de pagamento para
todas as suas contas.<br>
O Amazon Virtual Private Cloud (VPC) é um serviço que permite iniciar recursos da AWS
em uma rede virtual iSQLada logicamente definida por vocé.
https://aws.amazon.com/pt/?nc2=h_lg

#

## Pergunta 47: 

Qual é o serviço de alta performance desenvolvido para fornecer block-storage para
instáncias EC2?

- [X] EBS
- [ ] KMS
- [ ] ELB
- [ ] S3

### Explicação
**Correta**
desc
Eas - Elastic Block Store<br>
O EBS é um dos serviços que oferece armazenamento de dados para ser incorporado
instãncias EC2 e atender diversas finalidades computacionais, como sistema
operacional, banco de dados IaaS, etc.<br>
https://aws.amazon.com/ebs/?nc2=h_ql_prod_st_ebs&ebs-whats-new.sort-
by=item.additionalFields.postDateTime&ebs-whats-new.sort-order=desc

**Incorretas**

O KMS - Key Management Service - fornece chaves de criptografia pra vários serviços,
incluindo o EBS<br>
O ELB - Elastic Load Balancer - faz balanceamento de carga entre EC2<br>
O S3 - Simple Storage Service - é o serviço de storage padrão de objetos e arquivos.

#

## Pergunta 48: 

Vocé está migrando parte de uma aplicação que trabalha com sistema de arquivos para
armazenar e manipular alguns dados. Qual das opções abaixo indica o serviço que pode
ser utilizado para atender essa parte da aplicação na AWS?

- [ ] AWS Config
- [ ] KMS
- [X] EFS
- [ ] EC2

### Explicação
**Correta**

O EFS pode ser anexado a suas instãncias EC2 permitindo o uso de sistemas de arquivo.<br>
O mesmo EFS pode ser utilizado com diversas máquinas de acordo com a necessidade.
Oferece a maior e mais abrangente plataforma de computação com a possibilidade de
escolha de processador, armazenamento, rede, sistema operacional e modelo de compra
https://aws.amazon.com/efs/?nc2=h_ql_prod_st_efs

**Incorretas**

O Amazon Elastic Compute Cloud (Amazon EC2) é um serviG0 Web que disponibiliza
capacidade computacional segura e redimensionável na nuvem. Ele foi projetado para
facilitar a computação em nuvem na escala da web para os desenvolvedores.<br>
O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves
criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em
seus aplicativos.<br>
O AWS Config é um serviço que permite acessar, auditar e avaliar as configuraqóes dos
recursos da AWS. O Config monitora e grava continuamente registros das configuraqóes
de recursos da AWS e lhe permite automatizar a avaliação das configuraqóes registradas
com base nas configuraqóes desejadas

#

## Pergunta 49: 
O que é Free Tier (Nivel Gratuito)?

- [ ] E uma camada de banco de dados NoSQL
- [ ] E um servieo de firewall que protege suas aplicaqóes
- [ ] E um modelo open source (código aberto) para o desenvolvimento de aplicaqóes em camadas
- [X] E um modelo de uso onde vocé não é cobrado na AWS

### Explicação
**Correta**


E um modelo de uso onde vocé não é cobrado e que é apresentando em trés tipos:<br>
1) 12 meses de gratuidade,<br>
2) Sempre gratuito<br>
3) Experimentação.<br>
Há centenas de configuração de serviqo para uso gratuito, vale pena dar uma navegada
no site para visualizar as opções.
https://aws.amazon.com/pt/free/?all-free-tier.sort-
by—item.additionalFields.SortRank&all-free-tier.sort-

**Incorretas**

As demais opçóes não estão relacionadas ao nivel gratuito.<br>

*Nota*<br>
Ser for testar qualquer serviqo da AWS, configure o AWS Budget (Orgamento) para
notificar se a sua infraestrutura está consumindo algo que não é ou que não está mais
gratuito.<br>
Ele envia um e-mail se o custo ultrapassar um valor pré-definido por vocé. Isso
te auxilia no gerenciamento de custos e evita surpresas indesejáveis no seu cartão de
crédito.

#

## Pergunta 50: 
Qual é o serviqo serverless (sem servidor) que permite a execução de consultas
utilizando padrão SQL para analisar dados no Amazon S3?

- [ ] O EMR
- [X] Athena
- [ ] Amazon Elastic Search
- [ ] Amazon Query Analyzer

### Explicação
**Correta**

Com o AWS Athena vocé pode criar estruturas de dados para realizar queries
diretamente nos arquivos que estão no S3 e executá-las sem servidor.
https://aws.amazon.com/athena/?c=a&sec=srv&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc

**Incorretas**

O Amazon auery Analyzer não existe<br>
O Amazon ElasticSearch Service é um serviço totalmente gerenciado com o qual vocé
pode pesquisar, analisar e visualizar seus dados de log de maneira econámica, em escala
de petabytes<br>
O EMR é a plataforma para uso de Big Data

#
## Pergunta 51: 
O AWS Trusted Advisor é um serviqo de monitoramento e recomendação que auxilia o
cliente a utilizar os recursos de sua conta de maneira alinhada com as melhores práticas
para trazer muitos beneficios. Ouais itens abaixo representam tais beneficios? (Selecione 3)

- [X] Seguranga
- [X] Otimização de Custos
- [ ] Proteção de Hardware
- [X] Performance

### Explicação
**Correta**

O AWS Trusted Advisor faz recomendaqóes que te ajudam a seguir as práticas
recomendadas da AWS.<br>
O Trusted Advisor avalia a sua conta por meio de verificações.<br>
Essas verificações identificam formas de otimizar sua infraestrutura da AWS, aumentar a
segurança e o desempenho, reduzir os custos gerais e monitorar as cotas do serviqo.
https://aws.amazon.com/pt/premiumsupport/technology/trusted-advisor/

**Incorreta**

O Trusted Advisor não dá informações sobre o uso de Protecao de Hardware, umas vez
que isso não é responsabilidade do cliente e sim da AWS no modelo de responsabilidade
compartilhada.

#

## Pergunta 52: 

Utilização de recursos de rede, computadores virtuais e armazenamento de dados com
alto nivel de flexibilidade, gerenciamento e controle sobre os recurso de TI são
caracteristicas de qual tipo de uso de cloud?

- [X] IaaS
- [ ] SaaS
- [ ] PaaS
- [ ] BaaS

### Explicação
**Correta**

IaaS - Infraestrutura como serviqo.<br>
Neste tipo de uso, o cliente precisa gerenciar todos os recursos que precisa implementar
na cloud.<br>
Geralmente usa-se apenas instáncias EC2 e se configura-se todo o resto, instala-se
software, web hostings, bancos de dados, filas, etc..
https://aws.amazon.com/what-is-cloud-computing/?nc2=h_ql_le_int_cc

**Incorretas**

PaaS - Plataforma como serviqo - Neste modelo, o cliente sé precisa desenvolver o
software sobre a plataforma.<br>
SaaS - Software como serviço - Neste modelo, o cliente usa o software pronto.<br>
BaaS - Backend como servigo - Neste modelo, o cliente usa o backend e implementa
apensar o front-end.

#

## Pergunta 53: 

Vocé trabalha numa agéncia de viagens online e precisa armazenar, analisar e
correlacionar dados de logs de seus aplicativos para identificar e reSQLver gargalos de
desempenho e problemas de disponibilidade para garantir uma experiéncia de reserva
otimizada para os seus clientes. aual serviqo da AWS abaixo é o mais indicado?

- [ ] Amazon Cloud Search
- [ ] Amazon Athena
- [X] Amazon OpenSearch
- [ ] Amazon EMR

### Explicação
**Correta**

O Amazon OpenSearch é um conjunto distribuido, orientado comunidade, com licença
Apache 2.0 de pesquisa e análise de cédigo 100% aberto usado para uma ampla
variedade de casos de uso, como monitoramento de aplicaqóes em tempo real, análise
de logs e pesquisa de sites. O OpenSearch fornece urn sistema altamente escalável para
fornecer acesso ráPido e resposta a grandes volumes de dados com uma ferramenta de
visualização integrada.
https://aws.amazon.com/pt/opensearch-service/the-elk-stack/what-is-opensearch/

**Incorretas**

O CloudSearch oferece um serviqo de busca e localização para ser implementado no seu
website.<br>
O Athena é um serviqo servless que permite a consulta com SQL em buckets no S3.<br>
O EMR é a plataforma de BigData da AWS.
#

## Pergunta 54: 
Qual serviqo da AWS é recomendado para estimar o custo de implementação dos
serviços de Cloud para o seu neçõcio?

- [X] AWS Princing Calculator
- [ ] AWS Organizations
- [ ] AWS Cost Explorer
- [ ] AWS Billing

**Correta**

O AWS Princing Calculator pode ser utilizado pra estimar os custos antes do uso, antes
da implementação.
https://calculator.aws/#/

**Incorretas**

O AWS Cost Explorer tern uma interface fácil de usar que permite visualizar, entender e
gerenciar os custos e o uso da AWS ao longo do tempo. Relacionado ao que já foi gasto,
não pra estimar.https://aws.am<br>
O AWS Billing e Cost Management são o conjunto de serviqos que vocé usa para pagar o
faturamento, monitorar seu uso e analisar e controlar seus custos<br>
O AWS Organizations ajuda vocé a gerenciar e controlar seu ambiente de maneira
centralizada á medida que os neçõcios e seus recursos da AWS expandem. Usando o
AWS Organizations, vocé pode criar novas contas da AWS e alocar recursos, agrupar
contas para organizar seus fluxos de trabalho, aplicar politicas a contas ou grupos para
governanca e simplificar o faturamento usando um ünico método de pagamento para
todas as suas contas.
https://aws.amazon.com/pt/organizations/?nc2=type_a

#

## Pergunta 55: Incorreto
Vocé precisa automatizar um processo que executa diversas tarefas de forma sequencial
em seu sistema. Qual é o serviqo mais indicado para essa necessidade?

- [ ] AWS Workflow
- [ ] AWS EventBridge
- [ ] AWS Kinesis
- [X] AWS Batch

### Explicação
**Correta**

O AWS Batch possibilita que desenvolvedores, cientistas e engenheiros executem de
modo fácil e eficiente centenas de milhares de tarefas de computação em lote na AWS.<br>
O AWS Batch provisiona dinamicamente a quantidade e o tipo de recursos
computacionais ideais (por exemplo, instáncias otimizadas para CPU ou memória) com
base nos requisitos de volume e recursos especificos das tarefas em lote enviadas.
https://aws.amazon.com/batch/?nc2=h_ql_prod_cp_ba

**Incorretas**

O AWS Workflow não é um serviqo válido na AWS.<br>
O AWS Eventidridge é um barramento de eventos sem servidor que torna mais fácil a
criação de aplicaqóes orientadas por eventos em escala usando eventos gerados com
base em suas aplicaqóes, aplicaqóes integradas de software como serviqo (SaaS) e
serviqos da AWS - https://aws.amazon.com/pt/eventbridge/<br>
O AWS Kinesis é o serviqo utilizado para coletar uma grande quantidade de aplicativos
tranferindo para outros serviqos através de streaming.

#

## Pergunta 56: 
Quais das opções abaixo são formas de pagamento de instáncias EC2? (Selecione 3 alternativas)


- [X] Spot
- [ ] On premise (Próprio)
- [X] Reserved (Reservado)
- [X] On-demand (Sob demanda)
- [ ] Tailor Made (Sob demanda)

### Explicação
**Correta**

Existem cinco formas de pagar a Amazon EC2 instances:<br>
On-Demand, Savings Plans, Reserved Instances, Spot Instances, Dedicate Host.<br>

On-demand - paga somente pelo uso, recomendado quando ainda não se sabe a
quantidade de recursos necessários para uma aplicação. Tem alta disponibilidade e o
maior custo de todos as formas.<br>
Reserved - paga por um contrato pré-estabelecido, recomendado quando é possivel
estimar o uso por 1 ou 3 anos, Tem alta disponibilidade e economia de custo quando
comparado ao on-demand.<br>
Spot - paga pelo uso dos recursos não utilizados pelos outros modelos, recomendado
para processos que não precisam ser online, podendo ser executados apenas quando há
infraestrutura fica disponivel, não garante alta disponibilidades e o menor custo de todos
os meios.
https://aws.amazon.com/pt/ec2/pricing/

**Incorretas**

On premise é a infraestrutura própria, o data center privado da sua corporação, não está
relacionado a tipo de uso do EC2.<br>
Tailor Made - Sob Medida - esse tipo de uso não existe.

#

## Pergunta 57: 
Qual pilar do framework de melhores práticas arquitetónicas da AWS se concentra em
garantir que uma carga de trabalho execute sua função pretendida corretamente e de
modo consistente, e que uma carga de trabalho seja resiliente e que se recupere
rapidamente de falhas para atender a demanda do neçõcio e do cliente?

- [X] Confiabilidade
- [ ] Seguranga
- [ ] Excelência Operacional
- [ ] Performance Eficiente

### Explicação
Pilar de Confiabilidade<br>
https://aws.amazon.com/pt/architecture/well-architected/?achp_wal&wa-lens-
whitepapers. sort-by—item.additionalFields.sortDate&wa-lens-whitepapers.sort-
order—desc

Os 5 pilares são Excelência Operacional:<br>
**Segurança, Confiabilidade, Performance, Eficiente e Custo Otimizado.**

#

## Pergunta 58: 
Qual é o servico utilizado para permitir que aplicaqóes acessem recursos restritos de
serviqos dentro da AWS?

- [ ] IAM Users
- [X] IAM Roles
- [ ] IAM Groups
- [ ] IAM policies

### Explicação
**Correta**

Roles<br>
Todos os acessos entre aplicaqóes devem ser feitos através de uma Role configurada no
serviço IAM.<br>
Através de uma Role vocé associa policies e restricóes de acesso que podem ser
associadas a uma ou mais aplicaqóes.
https://docs.aws.amazon.com/lAM/latest/lJserGuide/id_roles.html

**Incorretas**

Todas as funções estão relacionadas ao IAM, que é utilizado para o gerenciamento de
usuários e recursos de uma conta Users para usuários, Groups para grupos de usuários,
Policies para restricóes para autorização ou negação de funcionalidades de servicos.

#
## Pergunta 59: Correto
Sua aplicação precisa persistir dados não estruturados de clientes. aual serviqo é o mais
indicado para essa finalidade?

- [X]  Amazon RedShift
- [ ]  Amazon DynamoDB
- [ ]  Amazon EMR
- [ ]  Amazon Aurora

### Explicação
**Correta**

O DynamoDB é um banco quer permite a gravação de registros com o conceito de chave
valor, onde o valor não precisa estar estruturado como em bancos de dados relacionais.

**Incorretas**

O Aurora é um banco de dados relacional e que precisar ser implementado de forma
estruturada<br>
O RedShit é um bando de dados de dados estruturado e semi-estruturado, mas o seu
usa é para finalidade de Bl (Business Inteligence)<br>
O EMR é a plataforma para BigData da AWS

#

## Pergunta 60: 
Qual é o serviço que permite estabelecer uma conexão dedicada entre a sua
infraestrutura on-premise e a AWS melhorando as conexóes e aumentando a taxa de
transferéncia?

- [X] AWS Direct Connect
- [ ] AWS DataSync
- [ ] AWS Link
- [ ] AWS API Gateway

### Explicação

**Correta**

O AWS Direct Connect faz uso da própria infraestrutura global da AWS para melhorar
esse tipo de conexão. O serviqo de nuvem é o caminho mais curto para seus recursos na
AWS. Seu tráfego de rede permanece todo o tempo na rede global da AWS e nunca entra
na Internet püblica. Isso reduz as probabilidades de gargalos ou aumentos inesperados
de laténcia
https://aws.amazon.com/pt/directconnect/

**Incorretas**

AWS Link não é um serviqo existente na plataforma.<br>
O Amazon API Gateway é um serviqo gerenciado que permite que desenvolvedores
criem, publiquem, mantenham, monitorem e protejam APIs em qualquer escala com
facilidade. APIs agem como a "porta de entrada" para aplicativos acessarem dados,
lógica de negócios ou funcionalidade de seus serviços de back-end<br>
O AWS DataSync é um serviqo de transferéncia de dados on-line que simplifica,
automatiza e acelera a movimentação de dados entre os sistemas de armazenamento
on-premises e os serviqos de armazenamento da AWS, e também entre serviqos de
armazenamento da AWS. Vocé pode usar o DataSync para migrar dados ativos para a
AWS, arquivar dados para liberar a capacidade de armazenamento on-premise, replicar
dados para a AWS para fins de continuidade de neçõcios ou transferir dados para a
nuvem para análises e processamento

#
## Pergunta 61: 
Qual é a SQLução de banco de dados em Grafo, gerenciado pela AWS, que permite
diversos tipos de relacionamentos entre os seus nás e que pode ser utilizado em muitos
contextos que representam as conexóes que temos em nosso cotidiano, como em rede
sociais, cadeias logisticas, empresariais, entre outros?

- [ ] Amazon Graph
- [X] Amazon Neptune
- [ ] Amazon JanusGraph
- [ ] Amazon Neo4j


### Explicação
**Correta**

O Amazon Neptune é um serviqo de banco de dados de grafos rápido, confiável e
totalmente gerenciado que facilita a criação e a execução de aplicativos.
https://aws.amazon.com/pt/neptune/

**Incorretas**

Apesar de serem em grafo, os demais banco de dados não são serviqos ofertados pela
AWS e para uso dos mesmos seria necessário o uso de uma infraestrutura IAAS, onde se
faz todo o gerenciamento dos servidores e realizar todas as instalaqóes e configuraqóes
necessárias, ou seja, pode-se instanciar uma máquina EC2 e instalar qualquer banco de
dados, mas que não será gerenciado pela AWS.

#

## Pergunta 62: 
Uma arquitetura de sistemas, baseada em computação sem servidor, utiliza S3, API
Gateway, Lambda, SOS, SNS e precisa de um serviqo que orquestre parte destas peqas
definindo e controlando os possiveis workflows. Qual dos serviços abaixo é utilizado para

- [ ] AWS Service Mesh
- [ ] AWS Workflow
- [X] AWS Step Functions
- [ ] AWS Even±Bridge

### Explicação
**Correta**

Com o AWS Step Function é possivel orquestrar e paralelizar vários serviqos da AWS
para executar um processo quando existirem todas as variáveis necessárias para isso.
Além disso tem uma interface gráfica que permite visualizar cada passo do workflow.
https://aws.amazon.com/step-functions/?c=ser&sec=srv&step-functions.sort-by=item.additionalFields.postDateTime&step-functions.sort-order=desc

**Incorretas**

O AWS Workflow e O AWS Service Mash não são servigos existentes na AWS. Existe o
AWS App Mesh que não está na lista, que é um service mesh que oferece redes para
aplicativos a fim de facilitar a comunicação dos serviqos entre si e entre vários tipos de
infraestrutura de computação<br>
O Amazon EventBridge é um barramento de eventos sem servidor que torna mais fácil a
criação de aplicaqóes orientadas por eventos em escala usando eventos gerados com
base em suas aplicaqóes, aplicaqóes integradas de software como serviqo (SaaS) e
serviqos da AWS.

#

## Pergunta 63:
Vocé está auditando a infraestrutura da sua empresa na AWS para tentar identificar
at;óes não programadas de desligamentos de recursos. Qual serviqo pode te auxiliar
nesta atividade?

- [ ] AWS CloudSearch
- [X] AWS CloudTrail
- [ ] AWS Cloud ElasticSearch
- [ ] AWS Audit

### Explicacão
**Correta**

O CloudTrail loga a chamada de todas as chamadas de API que são usadas para o
desligamento de recursos na infraestrutura da AWS

**Incorretas**

AWS Audit não é um serviqo válido na AWS<br>
AWS CloudSearch é um serviqo que permite a implementação de uma funcionalidade
busca dentro do seu site na AWS.<br>
AWS ElasticSearch é um serviqo para armazenar, analisar e correlacionar uma grande
quantidade de dados de logs de seus aplicativos para identificar e reSQLver gargalos de
desempenho e problemas de disponibilidade.<br>
OpenSearch é uma bifurcação do ElasticSearch e Kibana de código aberto, licenciada sob a ALv2 e orientada pela
comunidade.
https://aws.amazon.com/pt/opensearch-service/the-elk-stack/what-is-ElasticSearch/

#

## Pergunta 64: Incorreto
A sua empresa decidiu migrar algumas aplicaqóes monoliticas legadas, sem refatoração,
para o ECS. O que pode-se afirmar sobre essa estratégia?

- [ ] E possivel e recomendado
- [ ] E passivel e trarã mais veloeidade para a migragão e implementagão de novas funcionalidades.
- [ ] não é possivel, pois o servieo não aceita aplicaqóes monoliticas.
- [X] E possivel, porém não trarã grandes beneficios de otimizagão no uso dos recursos

### Explicação
**Correta**

E possivel, porém não trará grandes ganhos como uma SQLução em microsserviqos que
faz um gerenciamento melhor dos recursos da rnáquina de acordo com a demanda da
aplicação. A aplicação inteira vai ficar num ünico container.
https://aws.amazon.com/pt/getting-started/hands-on/break-monolith-app-
microservices-ecs-docker-ec2/module-one/

**Incorretas**

O ECS aceita a aplicação de acordo com a capacidade da infraestrutura utilizada, mas o
ideal é que a aplicação seja refatorada em microsserviqos para permitir o melhor uso dos
recursos, além de facilitar futuras evoluqóes e manutenqóes.

#

## Pergunta 65: 
Qual das opções abaixo é a classe que pode deixar o uso do S3 mais caro?

- [ ] Glacier
- [X] Standard
- [ ] Standard Infrequent Access
- [ ] Glacier Deep Arquive

### Explicação

**Correta**

O Standard oferece alta disponibilidade, durabilidade e tempo de recuperação, dessa
forma tem o maior prep. Algumas aplicaqóes não requerem um tempo de resposta tão
rápido, o que permite pensar em outras opções para diminuir o custo. Ex. arquivos
históricos, arquivos pouco utilizados.
https://aws.amazon.com/pt/s3/pricing/

**Incorretas**

As demais classes vão ficando mais baratas, na medida que os objetos são menos acessados em cada uma delas.<br>
Standard Infrequent Access.<br>
Glacier.<br>
Glacier Deep<br>
