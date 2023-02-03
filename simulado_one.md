## Pergunta 1: 
Oual serviço da AWS possui um catálogo onde os clientes podem encontrar aplicações
desenvolvidas porterceiros, prontas para serem instaladas e executadas para atender as
mais diversas necessidades de negócio?


- [ ] AWS AMI
- [X] AWS Marketplace
- [ ] AWS MFA
- [ ] AWS OpsWorks

Explicação

AWS Marketplace
Existem muitos tipos de aplicações e contextos de negócio para uso imediato.
Útil para comercializar alguma aplicação feita pelo cliente.
Essa pergunta é direta, porém, é importante pensar se poderia entrar em contextos onde
a sua empresa tem a necessidade de comprar alguma aplicação pronta para atender
alguma finalidade latente e especifica, cuja compra seja melhor que o desenvolvi mento.
https•Waws-amazon.com/marketpIace/?nc2=type_a

Incorretas
O AWS MFA - Multi Factor Authentication adiciona uma camada a mais no processo de
autenticação no login pelo Console
O AWS AMI - Amazon Machine Images (AMIs) são pré-configuraçaes de uma lista de
sistemas operacionais para a instalação instantânea em instâncias EC2
O AWS OpsWorks é um serviço de gerenciamento de configurações que oferece
instâncias gerenciadas do Chef e do Puppet. O Chef e o Puppet são plataformas de
automação que permitem usar cód igo para automatizar a configuração de servidores. O
OpsWorks permite usar o Chef e o Puppet para automatizar a forma como os servidores
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

Explicação
Correta
O AWS Certificate Manager permite a criação e gerenciamento de certificados digitais
que são utilizados para criptografar os dados entre os usuários e os servidores com base
no protocolo https tornando o tráfego de dados seguro. Quando certificados digitais não
são utilizados, dados de usuários, senhas, números de documentos e cartões de crédito,
etc são trafegados sem nenhuma segurança e podem ser expostos de forma indevida.
https://aws.amazon.com/certificate-manager/?nc2=type_a

Incorretas
AWS Cognito é um serviço que pode ser utilizado para fazer controle de acesso em
aplicações web e mobile, ofertando diversas funcionalidades para esse fim.
AWS IAM é o serviço utilizado para gerenciar acesso de usuário e serviços.
AWS KMS é o serviço utilizado para criar chaves de criptografia para uso em diversos
serviços da AWS, geralmente para dados, arquivos no S3.

#

## Pergunta 3: 
Você irá disponibilizar uma aplicação crítica e com dados sensíveis na Internet. Oual é o
serviço que te ajuda a identificar vulnerabilidades de segurança e riscos de exposição de
acordo com as melhores práticas e compliance?

- [X] O AWS Inspector
- [ ] O AWS Macie
- [ ] O AWS KMS
- [ ] O AWS GuardDuty

Explicação
Correta
O Amazon Inspector é um serviço automatizado de gerenciamento de vulnerabilidade
que verifica continuamente as workloads da AWS em busca de vulnerabilidades de
software e exposição não intencional à rede.
https://aws.amazon.com/inspector/Qnc2=type_a

Incorretas
O Amazon GuardDuty é um serviço de detecção de ameaças que monitora
continuamente atividades mal-intencionadas e comportamentos não autorizados para
proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon Sê.
O Amazon Macie é um serviço de rança e privacidade de dados totalmente
gerenciado que usa machine learning e correspondência de padrões para descobrir e
proteger seus dados confidenciais na AWS. À medida que as organizações gerenciam
volumes crescentes de dados, identificar e proteger seus dados confidenciais em escala
pode se tornar cada vez mais complexo, caro e demorado. O Amazon Macie automatiza a
descoberta de dados confidenciais em escala e reduz o custo da proteção de seus dados
O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves
criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em
seus aplicativos
https://aws.amazon.com/pt/kms/

#

## Pergunta 4: 

Sua empresa deseja otimizar o custo com a utilização do S3 e você notou que existem
muitas logs armazenadas e que poderiam ser deletadas após 30 dias da criação. O que
pode ser feito para essa otimização?

- [X] Configurar no S3 Lifecycle para que os objetos expirem em 30 dias para serem automaticamente excluídos.
- [ ] Criar uma cópia destes objetos em outra região
- [ ] Configurar o CloudWatch para monitorar o S3 e enviar um email solicitando a exclusão dos arquivos
- [ ] Criar uma cópia destes objetos em outra zona de disponibilidade

Explicação
Correta
Configurar a expiração dos objetos para serem excluídos de forma automática quando
vencerem.
https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html

Incorretas
As demais opções são formas de gerenciar e monitorar os objetos, não trazem redução
de custos

Pergunta 5: Incorreto

Sua empresa iniciou um processo de transformação digital de todas as suas plataformas
e decidiu utilizar uma arquitetura de sistemas orientada a eventos. Qual dos serviços
abaixo pode ser utilizado como um barramento escalável de eventos para facilitar a
criação dessa arquitetura?

- [ ] Amazon EventSync
- [ ] Amazon Lambda
- [ ] Amazon SQS
- [X] Amazon EventBridge*

Explicação
Correta
O EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação
de aplicações orientadas por eventos em escala usando eventos gerados com base em
suas aplicações, aplicações integradas de software como serviço (SaaS) e serviços da
AWS. Você pode configurar regras de roteamento para determinar para onde enviar seus
dados para criar arquiteturas de aplicações que reagem em tempo real às suas origens
de dados com o consumidor e editor de eventos completamente dissociados
https:Waws.amazon.com/pt/eventbridge/?nc2=h_ql_prod_ap_eb

Incorretas
O Lambda é utilzado para implementar funções sem servidores.
O SOS - Simple Queue Service é utilizado para enfileirar mensagens e desacoplar o
serviços dos sistemas
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

Explicação
O IP Elástico permite manter um IP ativo como porta de entrada e também que sejam
feitas associações de IPS dinâmicos a cada provisionamento de uma nova máquina, uma
vez que nesses cenários os IPV4 mudam.
https:Waws.amazon.com/pt/ec2/features/

#

## Pergunta 7: 
Oual é o banco de dados relacional totalmente gerenciado pela AWS e que pode ser 5 x
mais rápido que o MySQL?

- [ ] ManaDb
- [ ] Neptune
- [ ] DynamoDb
- [X] Aurora*

Explicação
O Amazon Aurora é um banco de dados compativel com MySQL e PostgreSOL criado
para a nuvem e que combina a performance e a disponibilidade de bancos de dados
empresariais tradicionais com a simplicidade e a economia de bancos de dados de
código aberto.
O Amazon Aurora é até cinco vezes mais rápido que bancos de dados MySOL padrão e
três vezes mais rápido que bancos de dados PostgreSOL padrão. O serviço oferece a
segurança, a e a confiabilidade de bancos de dados comerciais por um
décimo do custo. O Amazon Aurora é gerenciado pelo RDS, que automatiza tarefas
administrativas demoradas como provisionamento de hardware, configuração do banco
de dados, aplicação de patches e backups.
https://aws_amazon.com/pt/rds/aurora/?nc2=type_a&aurora-whats-new_sort-
by—item .add itio nal Fields. postDateTime&au rora-whats-new.sort-order=desc

Incorretas
O Neptune é um banco de dados totalmente gerenciado pela AWS, noSOL e baseado em
Grafos.
O DynamoDb é um banco de dados totalmente gerenciado pela AWS, noSOl„ baseado
em chave e valon
O MariaDb é um banco de dados totalmente gerenciado pela AWS quando utilizado no
RDS e não gerenciado quando instalado instalado diretamente numa instância EC2, é
relacional, não é 5 x mais rápido que o mySOL.

Nota
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

Explicação
O Standard está definido como padrão por oferecer diversas otimizações, usar as outras
opções sempre devem ser avaliadas de acordo com requisitos de qualidade da
aplicação, como tempo de resposta necessário, entre outros.
https:Waws.amazon.com/s3/storage-classes/?nc=sn&loc=3

Incorretas
As demais classes precisam ser configuradas e irão apresentar um tempo de resposta de
recuperação maior do que no modelo padrão.
Uma classe não citada e que pode ajudar na movimentação entre as classes de forma
automática é a Inteligente Tiering.

#

## Pergunta 9: 
Oual é o serviço que garante que você tenha o correto número de instâncias EC2
dis;xníveis para lidar com a carga da sua aplicação?

- [ ] Route53
- [X] EC2 Auto Scaling
- [ ] VPC
- [ ] ELB

Explicação
Correta
O Amazon EC2 Auto Scaling ajuda a manter a disponibilidade das aplicações e permite
adicionar ou remover instâncias do EC2 automaticamente de acordo com as condições
que você definir. É possível usar os recursos de gerenciamento de frota do EC2 Auto
Scaling para manter a integridade e a disponibilidade da sua frota Você também pode
usar os recursos de escalabilidade dinâmica e preditiva do EC2 Auto Scaling para
adicionar ou remover instâncias do EC2. A escalabilidade dinâmica responde às
mudanças na demanda e a escalabilidade preditiva agenda automaticamente o número
certo de instâncias do EC2 com base na demanda prevista
https://aws.amazoncom/pt/ec2/autoscaling/

Incorretas
O Amazon Route 5.3 é um web service DNS na nuvem altamente disponivel e escalável.
Ele foi projetado para oferecer aos desenvolvedores e empresas uma maneira altamente
confiável e econômica de direcionar os usuários finais aos aplicativos de Internet,
convertendo nomes como wwwexample.com para endereços IP numéricos como
192.0.2.t, usados pelos computadores para se conectarem entre si. O Amazon Route 53
também é totalmente compatível com 0 IPv6_
https•Waws.amazon.com/pt/route53/Pnc2=type_a

O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações
entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IR,
funções do Lambda e dispositivos virtuais. O serviço pode lidar com a carga variável de
tráfego das aplicações em uma única zona de disponibilidade ou em diversas zonas de
disponibilidade
https://aws.amazon.com/pt/elasticloadbalancing/?whats-new-cards-elb-sort-
bFitem .add itionalFields. postDateTime&whats- new-cards-elb. sort-order—desc

O AWS VPC - Virtual Private Cloud permite que você crie uma rede privada isolada para
alocar diversos recursos.

#

## Pergunta 10: 
Você implantou uma aplicação em produção que não está funcionando e na log existe
uma mensagem de acesso negado ao DynamoDB. Oual serviço você precisa checar e
configurar corretamente para validar esse acesso?

- [x] O AWS IAM roles
- [ ] O AWS IAM Policy
- [ ] O AWS Config
- [ ] O AWS Cognito

Explicação
Correta
(Correto)
Através de roles podemos gerenciar os acessos das aplicações aos serviços da AWS,
como o DynamoDB, RDS, entre outros.

Incorretas
AWS Config você gcde usar para gerenciar e monitorar as configurações dos seus
serviços

IAM Policy são as políticas relacionadas a cada serviços e que podem ser adicionadas a
pessoas ou roles, com uma série de permissões ou restrições

AWS Cognito é o serviço utilizado para fornecer autenticação para aplicações web e
mobile

#

## Pergunta 11: 

Quais dos seguintes planos de suporte oferecem acesso ao atendimento ao cliente,
whitepapers, documentações e fóruns de suporte 24x7? (Selecione 2)

- [x] *Basic*
- [ ] Full
- [x] *Enterprise*
- [ ] Reserved

Explicação

Corretas
Todos os planos desde o Basic oferecem esses serviços. Basic, Developer, Business,
Entrerprise on ramp e Enterprise.
Nas opções listadas só tem Basic e Enterprise e são as únicas possíveis pois as outras
não são planos de suporte existentes.
Para os planos business e enterprise existe uma opção de suporte técnico aprimorado
24x7, que é mais exclusivo e que dá acesso aos engenheiros da AWS por telefone e e-
mail, mas que só seria a resposta caso a pergunta estivesse relacionada a suporte
técnico aprimorado.
Maiores detalhes em: https://aws.amazon.com/premiumsupport/plans/

Incorretas
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

Explicação
Correta
O AWS X-Ray rastreia as solicitações do usuário enquanto percorrem todo o aplicativo.
Ele agrega os dados gerados por serviços e recursos individuais que compõem o
aplicativo, oferecendo uma visão completa do seu
desempenho.https://aws.amazon.com/pt/xray/?nc2=h_ql_prod_dt_xray

Incorretas
O AWS CloudSearch é um serviço que permite a implementação de um serviço de busca
dentro de uma aplicação.

AWS ElasticSearch é um serviço para armazenar, analisar e correlacionar uma grande
quantidade de dados de logs de seus aplicativos para identificar e resolver gargalos de
desempenho e problemas de disponibilidade. OpenSearch é uma bifurcação do
Elasticsearch e Kibana de código aberto, licenciada sob a ALv2 e orientada pela
comunidade.
https://aws.amazon.com/pt/opensearch-service/the-elk-stack/what-is-elasticsearch/

O AWS CloudWatch é utilizado para gerar métricas e monitorar diversos serviços e
aplicativos na AWS.


#

## Pergunta 13: 
Seu time de desenvolvimento identificou que um banco de dados relacional está com
baixa performance, a concorrência entre um grande volume de consultas e outras ações
na base de dados têm aumentando a latência no tráfego dos dados. Qual é a maneira
mais ágil e econômica de resolver este problema?

- [ ] Atualizar a role de acesso ao banco
- [ ] Criar novas instâncias do RDS em outra zona de disponibilidade.
- [ ] Substituir o RDS pelo Dynamo
- [x] Fazer o uso de Read Replicas

Explicação

Correta
Com o uso de Read Replicas você pode aumentar a escalabilidade e melhorar o tráfego
dos seus dados direcionando os processos somente de leitura para cópias das bases de
dados
https://aws.amazon.com/rds/features/

Incorretas
As roles de acesso a dados não tem nenhuma relação com performance, são serviços
que autorizam ou negam os acessos.
A substituição do banco de dados de um banco de dados relacionais (RDS) pelo
DynamoDB não é algo comum, uma vez que são banco de dados para usos diferentes e
esse tipo de estratégia exigiria grandes alterações do backend da aplicação.
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

Explicação
Correta
AWS Route53

Incorretas
Com RegistroCom, além do registro será necessário configurar o Route53
O EC2 não deve ser utilizado como servidor DNS público
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

Explicação

Correta
AWS CloudFormation
Arquivos Contendo o IAC, Infraestrutura como código, podem ser versionados e
atualizados de forma automatizada com o uso de CloudFormation
https://aws.amazon.com/pt/cloudformation/

Incorretas
AWS CodePipeline é utilizado para montar uma esteira de CI/CD para desenvolvimento
de aplicações

IAC é uma sigla utilizada para definir Infraestrutura como serviço, que é o que o
CloudFormation entrega, porém um serviço com o nome AWS IAC não existe.

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

Explicação
Estratégia Multi Region
https://aws.amazon.com/rds/features/read-replicas/
No link tem uma tabela comparando as 3 estratégias de implantações, Multi-AZ, Multi-Regiões e Read Replicas.

Multi-AZ é para aumentar a disponibilidade
Muti-Regiões para DR e Read Replicas para escalabilidade.

#

## Pergunta 17: 

Você deseja monitorar o percentual de memória que os seus servidores estão utilizando
em determinando período do dia. Qual serviço da AWS pode ser utilizado para essa
finalidade?

- [ ] AWS DataSync
- [x] AWS CloudWatch
- [ ] AWS Cost Explorer
- [ ] AWS CloudTrail

Explicação
Correta
Com o AWS CloudWatch você pode monitorar os recursos da sua infraestrutura

Incorretas
O CloudTrail pode ser utilizado para realizar logs de eventos relacionados a api de
serviços.

O Cost Explorer é para acompanhar os gastos da sua infraestrutura.

O DataSync realiza a transferência de dados de forma automatizada entre ambientes on
premise e AWS.

#

## Pergunta 18: 
Você está desenvolvendo uma aplicação mobile e precisa implementar o
armazenamento e sincronismo de dados para vários dispositivos. Qual é o serviço AWS
que pode ser utilizado para esse fim?

- [X] AWS Cognito
- [ ] AWS ElastiCache
- [ ] AWS DynamoDB
- [ ] AWS Redis

Explicação
Correta
Além de fornecer um serviço de autenticação robusto para aplicativos móveis, o Amazon
Cognito permite o salvamento de dados num banco local de chave-valor para depois
realizar o sincronismo.
https://aws.amazon.com/pt/cognito/getting-started/

Incorretas
O ElastiCache permite o armazenamento em memória para ser utilizados por aplicações
escaláveis para guardar informações de sessão, consultas de bancos de dados, entre
outros.

O Redis é ofertado pelo ElastiCache para prover cache de para as aplicações.

O DynamoDb é o banco de dados totalmente gerenciado pela AWS, NoSql de
chave/valor

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

Explicação

Correta
O Fargate adiciona a possibilidade de execução de contaiiner sem servidor ao ECS,
diminuindo a mão de obra relacionada a configuração de ambiente.
https://aws.amazon.com/fargate/?nc2=h_ql_prod_ct_far&whats-new-cards.sort-
by=item.additionaIFieIds.postDateTime&whats-new-cards.sort-order=desc&fargate-
blogs.sort-by=item.additional

Incorretas
O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado
de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente
aplicações conteinerizadas.

O Amazon Elastic Kubernetes Service (Amazon EKS) executa o plano de controle e
orquestração de containers com Kubernetes em várias zonas de disponibilidade, detecta
automaticamente e substitui nós do plano de controle com problemas de integridade e
oferece atualizações e aplicação de patches sob demanda e sem tempo de inatividade.

O Amazon Elastic Container Registry (Amazon ECR) é um registro de contêiner
totalmente gerenciado que facilita o armazenamento, o gerenciamento, o
compartilhamento e a implantação de imagens e artefatos de contêiner em qualquer
lugar

#

## Pergunta 20: 

Uma das formas de garantir a elasticidade e economia no uso do EC2 é mantendo os
arquivos de programas e de sistemas em recursos computacionais distintos. Oual
serviço pode ser utilizado para isso?

S3
O Git
CodeCommit
*O EBS*

Explicação
Correta
Numa implementação padrão do serviço EC2 é necessário definir o tipo de máquina que
irá processar as instruções, e o tipo de EBS para armazenar e persistir os dados. Isso
permite que o EC2 seja ligado e desligado de acordo com o uso e que os dados fiquem
salvos no EBS durante esses processos.
https:Waws.amazon.com/pt/ec2/faqs/

Incorretas
O Git é um aplicativo para fazer o gerenciamento e gestão de código fonte.

O CodeCommit é utilizado para gerenciar código fonte no modelo Git, semelhante ao
GitHub, GitLab, etc.

O S3 é utilizado para armazenar arquivos em forma de objeto (documento + metadado
do documento) em estruturas de Buckets.

#

## Pergunta 21: 
Você precisa implementar no seu site uma funcionalidade para realizar pesquisas em
todas as páginas e arquivos para facilitar a navegação e experiência do seus usuário.
Qual SAAS disponível na AWS fornece ferramentas robustas para cumprir essa finalidade
e que pode ser facilmente utilizada na sua aplicação?

Amazon CloudWatch
Amazon Athena
*Amazon CloudSearch*
Amazon OpenSearch

Explicação
Correta
Amazon CloudSearch
https://aws.amazon.com/pt/cloudsearch/?nc2=h_ql_prod_an_cs

Incorretas
O Athena é um serviço servless que permite a realização de consultas utilizando SQL em
Buckets do S3.

O OpenSearch é um conjunto distribuído, orientado à comunidade, com licença Apache
2.0 de pesquisa e análise de código 100% aberto usado para uma ampla variedade de
casos de uso, como monitoramento de aplicações em tempo real, análise de logs e
pesquisa de sites.

O CloudWatch permite oferece a geração de métricas e monitoramento para diversos
serviços e aplicações da AWS.

# 

## Pergunta 22: 
Qual é a melhor descrição para o conceito de tolerância a falha?

A habilidade de um sistema crescer e provisionar novos recursos para
continuar executando suas cargas de trabalho sem interrupção
A habilidade de um sistema nunca falhar
A habilidade de um sistema permanecer em funcionamento
mesmo se um dos seus componentes falhar.
A habilidade de um sistema exibir mensagens de falhas para os usuários.

Explicação
Correta
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

Incorretas
Nenhum serviço possui a habilidade de nunca falhar. Todo componente pode falhar em
hardwares, softwares, infraestrutura, redes e etc. Numa visão de tolerância a falhas não
pode-se contar com isso.
A habilidade do sistema provisionar mais recursos sob demanda (on demand) para
atender as cargas de trabalho adequadas é conhecida como escalabilidade.
A exibição de mensagens de erro podem ser requisitos de negócio ou requisitos de
qualidade e não tolerância a falhas. Junto com as logs dos componentes é conhecida
como observabilidade.

#

## Pergunta 23: 
Qual dos seguintes serviços de bancos de dados é totalmente gerenciado pela AWS?

SQL Server
MySql
MariaDB
*DynamoDB*

Explicação
O Amazon DynamoDB é um banco de dados de chave-valor NoSOL, sem servidor e
totalmente gerenciado, projetado para executar aplicações de alta performance em
qualquer escala.
Quando um serviço é totalmente gerenciado o cliente não precisa se preocupar com
nada que está relacionado a sua implementação, como instalação, atualizações da
infraestrutura. A AWS faz todo o gerenciamento e o cliente utiliza apenas as APIS destes
serviços para a criação das tabelas, gravação e recuperação dos dados. No caso do
Dynamo, o cliente faz o uso do console ou das APIS para realizar a maior parte das
tarefas, sem se preocupar com a instalação do banco.
https://aws.amazon.com/pt/dynamodb/?nc2=type_a

Incorretas
As demais opções são sistemas gerenciadores de bancos de dados que podem ser
utilizados juntos com o RDS e totalmente gerenciados pela AWS ou instalados no EC2 e
gerenciado pelo cliente.

Como as demais opções não falaram do RDS, não é possível afirmar se é gerenciado pela
AWS ou pelo cliente, desta forma, a opção correta é o DynamoDB.
Quando o cliente deseja gerenciar o banco, ele fica responsável por todo o processo de
instalação, atualizações, melhorias de performance, etc. Configura um modelo uso laaS
pois só está utilizando o servidor como infraestrutura.

#

## Pergunta 24: 
Qual é o serviço utilizado para provisionar Desktops utilizando Windows ou Linux?

EC2
Amazon WorkSpaces
Amazon Desktops
Amazon CLI

Explicação
Correta
Com o Amazon Workspaces é possível provisionar um grande número de máquinas
virtuais para uso como desktops.
https://aws.amazon.com/workspaces/?nc2=h_ql_prod_eu_wspa&workspaces-
blogs.sort-by=item.additionalFields.created

Incorretas
O EC2 - Elastic Compute Cloud - fornece instâncias de servidores com diversas
configurações e opções de processamento, memória e rede

O Amazon CLI - Command Line Interface é uma interface por linha de comando que
você pode instalar pra fazer uso no seu desktop

O Amazon Desktops não existe

#

## Pergunta 25: 

Quais são os cinco planos de suporte ofertados pela AWS?

Basic, Developer, Business, Advanced, Enterprise On-Ramp
Standard, Developer, Business, Enterprise, Enterprise On-Ramp
Bronze, Silver, Gold, Diamond, Ruby
*Basic, Developer, Business, Enterprise On-Ramp, Enterprise*

Explicação

Correta
Basic, Developer, Business, Enterprise On-Ramp e Enterprise.
E importante conhecê-los e explorar as características que os diferenciam também.
Cada um oferece um pacote de serviços e recomendações de acordo com o objetivo do
uso da AWS.
Recomendo a leitura desta página que mostra todo os detalhes:
https://aws.amazon.com/pt/premiumsupport/plans/

Nota: Publicado: Nov 24, 2021
A Amazon Web Services (AWS) anunciou a disponibilidade geral do Enterprise On-Ramp,
um novo nível de suporte entre os atuais Business e Enterprise para ajudar os clientes
que estão começando sua jornada na nuvem e precisam de orientação especializada
para crescer e otimizar na nuvem
https:Waws.amazon.com/pt/about-aws/whats-new/2021/11/enterprise-on-ramp-
general-availability/

Incorretas
Standard, Advanced, Bronze, Silver, Gold, Diamond, Ruby não existem na AWS.

#

## Pergunta 26: 
Baseado nos pilares de excelência operacional, segurança, confiança, performance
eficiente, sustentabilidade e otimização de custos, qual é o Framework que ajuda os
arquitetos cloud a construirem aplicações seguras, com alta performance, resilientes e
eficientes?

AWS Pillar
AWS CloudFormation
AWS Well-Architected
Framework .Net

Explicação
Correta
AWS Well-Architected é composto pelos 6 pilares citados na questão.
https://wa.aws.amazon.com/wat.pillars.wa-pillars.pt_BR.html

Incorretas
O AWS CloudFormation oferece uma forma fácil de modelar uma coleção de recursos
relacionados da AWS e de terceiros, provisioná-la com rapidez e consistência e gerenciar
todo o seu ciclo de vida mediante o tratamento da infraestrutura como código

O Framework.net e o AWS Pillar não são serviços da AWS.

#

## Pergunta 27: 
Qual opção descreve a função do serviço Elastic Load Balancer?

Instanciar uma nova máquina quando uma das máquinas apresenta falha
Criar um cluster de máquinas dentro da mesma zona de disponibilidade
Distribuir o tráfego de entrada entre instâncias em diferentes regiões
*Distribuir o tráfego de entrada entre suas instâncias*

Explicação
Correta
(Correto)
Distribuir o tráfego entre instâncias na mesma região, geralmente alocadas em mais de
uma zona de disponibilidade.
https://aws.amazon.com/search/?searchQuery=eIb
Incorretas
O ELB não é o responsável por instâncias uma nova máquina quando uma apresenta
falha, ele é o serviço que deixa de direcionar o tráfego para essa máquina e balanceia a
carga só entre as máquinas saudáveis e disponíveis.
Para o balanceamento de carga entre regiões, o mais adequado é usar alguma estratégia
do Route53, como geolocalização, Volume de tráfego, etc.
O ELB é utilizado para balancear as cargas em mais de uma zona de disponibilidade e
também não cria um cluster de máquinas, apenas direciona as cargas entre elas.

#

## Pergunta 28: 

Utilizando os serviços da AWS, qual é a sequência esperada numa pipeline de CI/CD?

CodeCommit, CodeBuild, CodeDeploy
CodeCommit, CodeDeploy, CodeBuild
CodeBuild, CodeCommit, CodeDepIoy
CodeBuiId, CodeDepIoy, CodeCommit

Explicação
Correta
Essa é uma sequência lógica numa esteira de desenvolvimento:
CodeCommit - Gerenciamento dos fontes através de funções do Git.
CodeBuild - Compilação e Testes automatizados.
CodeDeploy - Implantação.

Incorretas
As demais ordens não apresentam a sequência lógica da esteira.

Nota
Os serviços apresentados são orquestrados através do serviço CodePipeline, que é a
esteira que integra todos os serviços mencionados na questão.
https://aws.amazon.com/pt/codepipeline/

Em questões sobre ciclos de desenvolvimento também é possível encontrar a citação do
CodeStar, que é um serviço que permite o gerenciamento dos recursos do projeto,
pessoas, permissões e recursos de infraestrutura, CodePipeline e os demais. O CodeStar
também oferece modelos de projetos, que diminuem a necessidade de diversas
configurações e trazem muita agilidade para todo o processo de desenvolvimento de
uma aplicação.
https://docs.aws.amazon.com/pt_br/codestar/latest/userguide/welcome.html

#

## Pergunta 29: 
Numa migração de sistemas, você percebeu que existem dados na sua aplicação que
raramente são usados e que poderiam ser mantidos em arquivos somente para fins de
auditoria. Qual é o serviço da AWS que pode ser utilizado para esse objetivo com o
menor custo possível?

S3 Standard
*S3 Glacier*
S3 Infrequent Access
S3 Intelligent Tiering

Explicação
Correta
O Serviço S3 Glacier permite fazer a guarda destes dados de uma forma mais
econômica, porém com um tempo de recuperação mais lento.
https://aws.amazon.com/pt/glacier/faqs/

Incorretas
O S3 Standard oferece um armazenamento de objetos com altos níveis de resiliência,
disponibilidade e performance para dados acessados com frequência. O custo é maior
que o Glacier.

S3 Intelligent Tiering é a única classe de armazenamento em nuvem que oferece
economia automática de custos de armazenamento quando os padrões de acesso a
dados mudam, sem impacto na performance ou sobrecarga operacional. O custo é maior
que o Glacier.

O S3 Standard-IA é indicado para dados acessados com menos frequência, mas que
exigem acesso rápido quando necessários. O custo é maior que o Glacier.

#

## Pergunta 30: 
Você trabalha numa agência de publicidade que deseja implantar um site com o
conteúdo estático para fazer a primeira divulgação de um produto. Qual é o serviço da
AWS mais indicado para esse cenário?

EC2
Docker
*S3*
EFS

Explicação
Correta
O S3 permite o armazenamento de objetos como arquivos htlm, js, cs eliminando a
necessidade de uso do EC2 trazendo muito mais economia, disponibilidade e resiliência
para as suas soluções.

Incorretas
O EFS - Elastic File System é um serviço utilizado para implementar um serviço de
arquivos na sua arquitetura associado a instâncias EC2. Apesar de servir para armazenar
arquivos estáticos não é o mais fácil e barato de implementar.

O EC2 - Elastic Computing Cloud oferece diversas configurações de máquinas para
computação, associado a um EBS ou EFS poderia manter páginas web, entretanto não é
a forma mais barata e ágil.
O Docker é utilizado para microserviços e sua implementação na AWS é possível através
do ECS - Elastic Container Service.

#

## Pergunta 31: 
Qual afirmação abaixo NÃO se refere ao AWS Lambda?

*Permite o gerenciamento total dos recursos de infraestrutura*
Processa dados sem servidor
Pode ser acionado diretamente pelo AWS S3
Pode ser acionado diretamente pelo AWS SNS

Explicação
Lambda é totalmente gerenciado pela AWS e faz o provisionamento automático para
executar as funções.
E importante ter atenção com questões que tem uma negação (NÃO) no início pois
podem inverter as respostas que parecem óbvias.
https://aws.amazon.com/pt/lambda/?nc2=h_ql_prod_serv_lbd


#

## Pergunta 32: 
Qual é o usuário utilizado para acessar o AWS Console pela primeira vez e que possui
acesso a todos os recursos da conta? (Não sendo recomendado para uso no dia a dia.)

AWS IAM
AWS full user
*AWS account root user*
AWS Administrator

Explicação
Correta
O root user é informado no primeiro acesso da sua conta e só é recomendado para as
primeiras configurações dos demais acessos, uma vez que ele possui acessos ilimitados
a todos os serviços da conta.
https:Wdocs.aws.amazon.com/lAM/latest/UserGuide/introduction.html

Incorretas
Full User e Administrador não são conceitos utilizados nestes acessos.
O AWS IAM é o serviço utilizado para gerenciar os usuários, roles e serviços, não é o
usuário em si.

# 

## Pergunta 33: 
Sua aplicação fornece dados através de APIS REST para diversas aplicações diferentes.
Pensando num cenário de futuras manutenções e evoluções dos seus serviços, qual
opção abaixo pode melhor auxiliar a sua arquitetura a manter várias versões da mesma
API sendo executadas simultaneamente e não exigir que todos os consumidores
realizem adequações nas chamadas ao seu serviço?

AWS Zuul
AWS Route53
AWS EventBridge
*API Gateway*

Explicação
Correta
O API Gateway permite esse tipo de convivência
https://aws.amazon.com/pt/api-gateway/features/

Incorretas
O AWS Zuul não existe

O AWS EventBridge é um barramento de eventos sem servidor que torna mais fácil a
criação de aplicações orientadas por eventos em escala usando eventos gerados com
base em suas aplicações, aplicações integradas de software como serviço (SaaS) e
serviços da AWS.

O AWS Route53 é um web service Domain Name Server(DNS) na nuvem altamente
disponível e escalável

#

## Pergunta 34: 
O que é o MFA - Multi-Factor-Authentication (Autenticação Multi Fator)?

Um serviço que permite a conexão entre a máquina do cliente e um servidor na AWS através de um arquivo contendo key pairs (par de chaves)
*Um serviço que inclui uma etapa a mais no processo de autenticação de acesso a conta da AWS através do Console Web*
Um serviço para permitir que instâncias EC2 acessem banco de dados DynamoDb
Um serviço que utiliza key pairs (par de chaves) na autenticação do usuário através da CLI (Linha de Comando)

Explicação
Correta
Um serviço que inclui uma etapa a mais no processo de autenticação de acesso a conta
da AWS através do Console Web. Autenticação Multi Fator deve ser habilitada com algum
dispositivo de terceiros para a proteção do acesso via console. Um exemplo é o Google
Authenticator, que gera um código numérico a cada minutos que deve ser utilizado no
login.
https://docs.aws.amazon.com/pt_br/lAM/latest/UserGuide/id_credentials_mfa.html

Incorretas
Um serviço para permitir que instâncias EC2 acessem banco de dados DynamoDb são
roles (funções) definidas no IAM.

Um serviço que permite a conexão entre a máquina do cliente e um servidor na AWS
através de um arquivo contendo key pairs (par de chaves) é uma conexão SSH.

Um serviço que utiliza key pairs (par de chaves) na autenticação do usuário através da
CLI (Linha de Comando) é um processo de autenticação entre o cliente e AWS digitando
tais informações na linha de comando.

Nota
Além do processo de login, o MFA pode ser utilizado em outros processos, como:
- Deleção de bucktes do S3
- Login pelo Cognito para usuários finais em aplicações web e mobile

#

## Pergunta 35: 
Analise os serviços abaixo:
O primeiro serviço permite que aplicativos enviem mensagens críticas, em termos de
tempo, para vários assinantes através de um mecanismo de "push", eliminando a
necessidade de verificar periodicamente ou *pesquisar" por atualizações.

O segundo é um serviço de fila de mensagens, usado por aplicativos distribuidos para
trocar mensagens através de um modelo de sondagem e pode ser usado para
desacoplar componentes de envio e recebimento.
Qual é a sequência abaixo que informa corretamente os dois serviços?

SQS e SNS
SES e SNS
*SNS e SQS*
SES e SQS

Explicação
Correta
SNS - Simple Notification Service
O Amazon Simple Notification Service (Amazon SNS) é um serviço de mensagens
totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de
aplicação para pessoa (A2P).
https://aws.amazon.com/pt/sns/?whats-new-cards.sort-
by—item ditio nal Fields. postDateTime&whats- new-cards.so rt-orde r=desc

SQS - Simple Oueue Service
O Amazon Simple Oueue Service (Amazon SOS) oferece uma fila hospedada segura,
durável e disponível que permite integrar e desacoplar sistemas de software e
componentes distribuídos
https://docs.aws.amazoncom/pt_br/AWSSimpleOueueService/latest/SOSDeveloperGui
de/welcome. html

Incorretas
As demais opções estão incorretas
O SES - Simple Email Service é utilizado para fazer envio de emails.