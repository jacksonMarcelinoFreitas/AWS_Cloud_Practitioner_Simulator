# Simulado AWS Cloud Practitioner 3/5 

## Pergunta 1: 
Qual item abaixo é de responsabilidade dos clientes quando é preciso garantir que dados
em volumes EBS estejam seguros e com seus backups realizados?

- [X] Criar a EBS snapshot
- [ ] Deletar o dado quando o dispositivo é destruído
- [ ] Anexar volumes em instâncias EC2
- [ ] Criar copias dos EBS Volumes

### Explicação

**Correta**

Para realizar o backup de dados que estão em volumes do EBS é necessário que o
cliente faça uma snapshot do mesmo, muitas vezes, em outras regiões para garantir a
segurança dos backups.<br>
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-creating-snapshot.html

**Incorretas**

A substituição e destruição de dispositivos é de responsabilidade da AWS.<br>
Cópias do EBS não são recomendadas para backups.<br>
Anexar novos volumes em instâncias EC2 não é permitido.<br>

#

## Pergunta 2: 

Para atender uma área de auditoria e compliance, você precisa garantir que as
configurações iniciais dos serviços e sistemas sejam mantidas e monitoradas. Qual
serviço da AWS você pode utilizar para esse tipo de gerenciamento?

- [ ] AWS Audit
- [ ] AWS Compliance
- [ ] AWS setup
- [X] AWS Config 

### Explicação

**Correta**

O AWS Config avalia, audita e avalia continuamente as configurações e os relacionamentos de seus recursos.<br>
https://aws.amazon.com/config/?nc2=h_ql_prod_mg_con

**Incorretas**

Os outros três serviços não existem na AWS

#

## Pergunta 3: 

O desenho dos dados da sua aplicação inclui uma base de dados relacional, que será
usada pontualmente e de forma imprevisível uma vez que você utilizará também o AWS
Elastic Cache para reduzir o acesso aos dados. Qual é o tipo de Instância de banco de
dados recomendado pra você ter mais economia neste contexto?

- [ ] Dedicated Hosts
- [ ] Reserved
- [X] On Demand
- [ ] Spot

### Explicação

**Correta**

O Sob demanda (on Demand) é cobrado por hora, indicado quando não é possível
estimar o custo para cargas desconhecidas.
https://aws.amazon.com/rds/mysql/pricing/?nc=sn&loc=4

**Incorretas**

Reserved (Reservada) - indicado para casos onde é possível prever o uso em períodos de
1 ou 3 anos permitindo a contratação antecipada. Apresenta maior economia comparado
ao Sob demanda.<br>
Spot - Indicado para casos onde é permitido que o processo seja interrompido e não
precise de alta disponibilidade, sendo executado quando algum recurso estiver
disponível. Apresenta maior economia comparado aos demais modelos.<br>
Dedicated Host (Hosts Dedicados) - Indicado quando é necessário utilizar uma máquina
física de maneira exclusiva Delo cliente.

#

## Pergunta 4: 
Qual conhecimento o seu time precisa para criar aplicações que façam uso do banco de
dados DynamoDB?

- [X] API do serviço e o Json com atributos e comandos
- [ ] GraphQl
- [ ] Athena
- [ ] Comandos SQL

### Explicação

**Correta**

Dado que o DynamoDB é um banco de dados totalmente gerenciado pela AWS, sua
utilização pode ser feita através de Apis e payloads em Json.<br>
https://docs.aws.amazon.com/amazondynamodb/latest/APlReference/Welcome.html

**Incorretas**

O Athena é utilizado para realizar consulta nos Buckets do S3.<br>
SQL é utilizado para realizar consulta em bancos relacionais.<br>
GraphOl para uso com banco de dados em Grafos

#

## Pergunta 5: 
Qual dos itens abaixo não faz parte dos tipos de uso Free Tier (nível gratuito)?

- [ ] 12 Meses gratuitos
- [ ] Testes - Experimentação (Trial)
- [ ] Sempre gratuito
- [X] Reserved

### Explicação

**Correta**

Reserved não é um nível gratuito, é um modelo de pagamento de instâncias EC2.

**Incorretas**

Os demais são níveis gratuitos que ofertam diversos serviços para serem usados
gratuitamente de acordo com a sua necessidade de uso, testes e experimentação.<br>
https://aws.amazon.com/pt/free/?all-free-tier.sort-by=item.additionalFields.SoftRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all

#

## Pergunta 6: 
Qual das seguintes opções deve ser configurada para que uma função Lambda escreva
dados no DynamoDB?

- [ ] SNS
- [X] IAM Roles
- [ ] API Gateway
- [ ] IAM Users

### Explicação

**Correta**

Para qualquer aplicação acessar serviços da AWS é necessária a criação e
gerenciamento de Roles com as permissões necessárias.<br>
IAM Roles - https://aws.amazon.com/iam/features/manage-roles/

**Incorretas**

O SNS Simple Notification Service é utilizado para troca de mensagens através do
processo de Pub/Sub e utilização de Tópicos.<br>
O API Gateway é utilizado para o gerenciamento e publicação de APIs.<br>
O IAM Users é utilizado para fazer o gerenciamento de usuários de uma conta.

#

## Pergunta 7: Correto
Sua empresa deseja implementar testes automatizados na sua esteira de
desenvolvimento, qual é o serviço da AWS que pode ser adotado para essa finalidade?

- [X] AWS CodeBuild
- [ ] AWS CodeDeploy
- [ ] AWS CodeTest
- [ ] AWS CodePipeline

### Explicação

**Correta**

AWS CodeBuild serve para compilar e realizar os devidos testes
https://aws.amazon.com/pt/codebuild/?nc2=type_a

**Incorretas**

O AWS CodePipeline é um serviço gerenciado de entrega contínua que ajuda a
automatizar pipelines de liberação para oferecer atualizações rápidas e confiáveis de
aplicativos e infraestruturas <br>
O AWS CodeDeploy é um serviço totalmente gerenciado de implantação que automatiza
implantações de software em diversos serviços de computação como Amazon EC2, AWS
Fargate, AWS Lambda e servidores locais <br>
O AWS CodeTest é um serviço que não existe na AWS.

#

## Pergunta 8: 
Você precisa implementar na sua conta, uma forma de facilitar a liberação de acessos
para o seu time de desenvolvimento e para colaboradores que ingressarem nele. Como
você pode realizar isso?

- [X] Fazendo uso do AWS IAM Grupos para criar um grupo de desenvolvedores e para fazer a gestão de acessos.
- [ ] Fazendo uso AWS Federation para criar um grupo de desenvolvedores e para fazer a gestão de acessos.
- [ ] Fazendo o uso de Roles para criar um grupo de desenvolvedores e para fazer a gestão de acessos.
- [ ] Fazendo o uso da AWS SDK que permite o gerenciamento de todos os desenvolvedores de forma automática

### Explicação

**Correta**

O AWS IAM Grupos permite que você crie grupos para gerenciar melhor e de forma mais
ágil a liberação de acesso a determinados perfis de colaboradores. <br>
Ex. Time de desenvolvimento, Time Devops, Time de Arquitetos, Time de Dbas, etc.
https://docs.aws.amazon.com/pt_br/lAM/latest/lJserGuide/id_groups.html

**Incorretas**

Acessos Federados (Federation) são utilizados para integrar processos de autenticação
de terceiros com a AWS. Ex. Google, Facebook, Apple, etc.
Funções (Roles) são tipos de identidades criados no IAM para que as aplicações ou
serviços possam recebem autorização para acessar outras aplicações ou serviços.
O AWS SDK é uma plataforma de desenvolvimento que acelera o processo de
desenvolvimento de software na AWS, apesar disso, o acesso tem que ser concedido
pelo IAM.

#

## Pergunta 9: 
Qual é o documento que fornece uma declaração formal de uma ou mais permissões no IAM?

- [ ] Users
- [ ] Role
- [X] Policies
- [ ] Groups

### Explicação

**Correta**

Policies ou Políticas de Pemissão.<br>
Você gerencia o acesso na AWS criando políticas e anexando-as às identidades do IAM
(usuários, grupos de usuários ou funções) ou aos recursos da AWS. Uma política é um
objeto na AWS que, quando associado a uma identidade ou um recurso, define suas
permissões. A AWS avalia essas políticas quando uma entidade de segurança do IAM
(usuário ou função) faz uma solicitação. As permissões nas políticas determinam se a
solicitação será permitida ou negada.<br>A maioria das políticas são armazenadas na AWS
como documentos JSON<br>
https://docs.aws.amazon.com/pt_br/lAM/latest/lJserGuide/access_policies.html

**Incorretas**

As demais opções estão relacionadas a gestão de acessos, mas possuem finalidades
diferentes.

#

## Pergunta 10: 
Qual é a principal função do Security Group?

- [ ] É servir apenas para agrupar recursos dentro de uma rede privada
- [ ] É proteger os data centers físicos da AWS
- [ ] É proteger a infraestrutura global da AWS de ataques de hackers
- [X] *E servir como uma espécie de firewall para controlar a autorização do tráfego de entrada e saída de máquinas EC2 que estejam associados a ele.*

### Explicação

**Correta**

O Security Groupe é uma espécie de firewall para as máquinas de uma VPC, você pode
utilizá-lo para agrupar diversas máquinas com a mesma função como, banco de dados,
aplicação, também pode ser utilizada no lançamento de novas máquinas para receber as
mesmas configurações de entrada e saída de dados do grupo.
https://aws.amazon.com/vpc/details/

**Incorretas**

A proteção física da AWS e da infraestrutura global é de responsabilidade da AWS.
O security group tem a finalidade de agrupar os servidores com o intuito de controlar o
tráfego de entrada e saída de dados.

#

## Pergunta 11: 
Você está desenvolvendo um serviço para enviar diariamente e-mails de aniversário para
mais de 1000 clientes. Qual é o serviço ofertado pela a AWS que pode se integrar a
qualquer aplicação para atender a esse requisito?

- [ ] AWS EventBridge
- [ ] AWS SNS
- [ ] AWS CloudWatch
- [X] *AWS SES*

### Explicação

**Correta**

O SES é o serviço recomendado para o envio de emails na AWS
https://aws.amazon.com/pt/ses/?nc2=h_ql_prod_ce_ses

**Incorretas**

O SNS é o serviço utilizado para troca de mensagens no esquema Pub/Sub e utilização
de tópicos
O EventBridge é um barramento de eventos que pode se utilizado para diversos serviços
e aplicações na AWS
O CloudWatch para coletar métricas, monitorar serviços e gerar log de aplicações

#

## Pergunta 12: 
Qual plano de suporte abaixo oferece acesso aos engenheiros do Cloud Support por
telefone, e-mail e chat 24 horas por dia, 7 dias por semana?

- [ ] Standard
- [ ] Basic
- [ ] Developer
- [X] Business

### Explicação

**Correta**s

Os planos existentes são
Basic, Developer, Business, Enterprise on-Ramp e Enterprise.
(Correto)
Esse tipo de suporte só é oferecido para os planos recomendados para cargas de
produção, o Business, Enterprise on-Ramp e Enterprise
https://aws.amazon.com/pt/premiumsupport/plans/?nc=sn&loc=l

**Incorretas**

Standard não é um nome válido para os planos de suporte ofertados pela AWS.

#

## Pergunta 13: 
Quais dos seguintes serviços permitem a criação de scripts e automação a partir da linha
de comando?

- [ ] AWS Run
- [ ] AWS Console
- [ ] AWS SDK
- [X] AWS CLI

### Explicação

**Correta**

A Interface da Linha de Comando (ILC ou mais comum em inglês CLI) da AWS é uma
ferramenta unificada para o gerenciamento de seus serviços da AWS. Com apenas uma
ferramenta para fazer download e configurar, você poderá controlar vários serviços da
AWS pela linha de comando e automatizá-los usando scripts.
https://aws.amazon.com/pt/cli/

**Incorretas**

AWS Console Management é o serviço que você usa para acessar e gerenciar a Nuvem
AWS, em uma única interface webAWS
SDK simplifica o uso do AWS Services, fornecendo um conjunto de ferramentas e
bibliotecas consistentes e familiares para os desenvolvedores
AWS Run é um serviço que não existe na AWS

#

## Pergunta 14: 
Qual é a melhor maneira de manter aplicações resilientes na infraestrutura AWS?

- [ ] Distribuir as instâncias em duas VPCs diferentes e dentro da mesma zona de disponibilidade
- [ ] Fazer uso do CloudFront
- [X] Distribuir as instâncias em mais de uma zona de disponibilidade
- [ ] Utilizar o Auto Scaling para subir uma máquina sempre que a outra cair

### Explicação

**Correta**

As boas práticas orientam a espalhar os recursos em zonas de disponibilidade
diferentes. Se ocorrer problema numa das zonas, as outras devem estar ativas para
responderem as demandas da aplicação com o mínimo impacto possível.

**Incorretas**

Distribuir as instâncias em duas VPCs diferentes e dentro da mesma zona de
disponibilidade não garante a resiliência, se a AZ ficar indisponível, as duas VPCs
também ficarão e impactarão a aplicação.
Fazer uso do CloudFront ajuda a melhorar a performance na distribuição de conteúdo, se
a origem da informação estiver numa única AZ e a mesma ficar indisponível, mesmo
como o uso do CloudFront, a aplicação poderá ser impactada.
Utilizar o Auto Scaling para subir uma máquina sempre que a outra cair garante que um
recurso esteja disponível, entretanto, se estiver numa única AZ que apresenta problema,
corre o risco de ficar indisponível.

#

## Pergunta 15: 
Você é uma pessoa desenvolvedora e gostaria de acessar os serviços da AWS
diretamente da sua IDE(lntelliJ, Visual Code, Eclipse, etc..). Qual serviço oferece uma
ferramenta (toolkit) para ser baixada e instalada na sua estação de trabalho e que
permita tal integração?

- [ ] AWS CLI
- [ ] AWS Console Manager
- [ ] AWS Workspaces
- [X] AWS SDKs

### Explicação

**Correta**

Com o AWS SDKs, você acessa e gerencia serviços da AWS com sua linguagem ou
plataforma de desenvolvimento preferida.
SDKs de mobilidade - Web e Plataforma Móvel
SDKs para dispositivos IOT
IDE e Kits de ferramentas de IDE
Ferramentas da linha de comando
Ferramentas do desenvolvedor da AWS
Linguagens: JavaScript, Python, Java, C#, PHP, Node, .Net, etc.
https://aws.amazon.com/pt/getting-started/tools-sdks/?nc2=type_a

**Incorretas**

O AWS workspaces oferece desktops virtuais windows e linux para de acordo com a
necessidade.
O AWS Console Manager é a interface web utilizada para gerenciar todos os serviços da
AWS.
O AWS CLI é o serviço utilizado para acessar e gerenciar os serviços da AWS através da
linha de comando.

#

## Pergunta 16: 
Qual dos serviços abaixo é uma solução para a criação de conteiners na AWS?

- [ ] ECR
- [ ] Auto Scaling
- [X] ECS
- [ ] EC2

### Explicação

**Correta**

ECS - Elastic Conteiner Service
https://aws.amazon.com/ecs/?whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc&ecs-
blogs.sort-by=item.additionalFields.createdDate&ecs-blogs.sort-order=desc

**Incorretas**

O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza
capacidade computacional segura e redimensionável na nuvem
O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade
para manter um desempenho constante e previsível pelo menor custo possível.
O Amazon Elastic Container Registry (Amazon ECR) é um registro de contêiner
totalmente gerenciado que facilita o armazenamento, o gerenciamento, o
compartilhamento e a implantação de imagens e artefatos de contêiner em qualquer
lugar

#

## Pergunta 17: 
Qual é o serviço que através das melhores práticas, pode ser utilizado para te ajudar a
identificar vulnerabilidades e desvios de segurança em aplicativos, antes de serem
implantados ou enquanto estiverem em execução em ambiente de produção?

- [ ] AWS WAF
- [ ] AWS Trusted Advisor
- [ ] AWS GuardDuty
- [X] AWS Inspector

### Explicação

**Correta**

AWS Inspector
https://aws.amazon.com/pt/inspector/?nc2=h_ql_prod_se_in

**Incorretas**

O AWS Trusted Advisor te auxilia checando o ambiente e te indicando as melhores
práticas de implementação
O Amazon GuardDuty é um serviço de detecção de ameaças que monitora
continuamente atividades mal-intencionadas e comportamentos não autorizados para
proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon S3
https://aws.amazon.com/pt/guardduty/?nc2=type_a
O AWS WAF é um firewall de aplicações Web que ajuda a proteger suas aplicações Web
ou APIS contra bots e exploits comuns na Web que podem afetar a disponibilidade,
comprometer a segurança ou consumir recursos em excesso.
https://aws.amazon.com/pt/waf/?nc2=type_a

#

## Pergunta 18: 
Após validar alguns cenários, sua empresa não autorizou o uso de computação
compartilhada, mas gostaria de encontrar uma solução da AWS que apresente as
mesmas características de simplicidade, agilidade e elasticidade e que faça uso de
servidores físicos dedicados. Qual é o serviço que pode atender essa necessidade?

- [ ] EC2 dedicados
- [ ] Hosts reservados
- [X] Hosts dedicados
- [ ] EC2 reservados

### Explicação

**Correta**

Hosts dedicados oferece essas características
https://aws.amazon.com/pt/ec2/dedicated-hosts/

**Incorretas**

Hosts reservardos e EC2 dedicados não existem
O EC2 pode ser utilizado com o meio de pagamento Reserved, onde é possível reservar
as instâncias necessárias por um período de 1 a 3 e ter uma economia de
aproximadamente 72% se comparado ao meio OnDemand, entretanto é uma forma
virtualizada e consumir os serviços de infraestrutura e não atenderia o requisito acima.

#

## Pergunta 19: 
Sua empresa precisa implementar mais segurança em seus recursos na AWS. Qual é o
serviço que permite provisionar, gerenciar e implantar facilmente certificados Secure
Sockets Layer (SSL)/Transport Layer Security (TLS) para que sejam usados com os
serviços da AWS e os recursos internos conectados?

- [ ] AWS KMS
- [ ] AWS Security
- [ ] AWS Protocols
- [X] *AWS Certificate Manager*

### Explicação

**Correta**

Certificate Manager
https://aws.amazon.com/pt/certificate-manager/?nc2=h_ql_prod_se_cm

**Incorretas**

AWS Protocols e Security não são serviços ofertados pela AWS.
O AWS KMS - Key Management Service é utilizado para criar chaves de criptografia para
diversos serviços mas não é indicado para SSL/TSL

#

## Pergunta 20: 
Você tem uma aplicação hospedada no EC2 que precisa enviar notificações para outras
aplicações e serviços baseadas em eventos. Qual dos serviços abaixo é o mais indicado
para essa necessidade?

- [ ] CloudWatch
- [ ] SES
- [ ] SQS
- [X] SNS

### Explicação

**Correta**

SNS - Simple Notifcation Service é um serviço de mensagens totalmente gerenciado
para a comunicação de aplicação para aplicação e de aplicação para pessoa.
A funcionalidade pub/sub de aplicação para aplicação fornece tópicos para sistemas de
mensagens de alta taxa de transferência baseados em push e de muitos para muitos
entre sistemas distribuídos, microsserviços e aplicações sem servidor orientadas por
eventos. Usando tópicos do Amazon SNS, seus sistemas editores podem repassar
mensagens para um grande número de sistemas de assinantes, incluindo filas do
Amazon SQS, funções do AWS Lambda e endpoints HTTPS e o Amazon Kinesis Data
Firehose para processamento paralelo.
https://aws.amazon.com/pt/sns/?whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc

**Incorretas**

O Amazon Simple Oueue Service (SQS) é um serviço de filas de mensagens gerenciado
que permite o desacoplamento e a escalabilidade de microsserviços, sistemas
distribuídos e aplicações sem servidor. O SOS elimina a complexidade e a sobrecarga
associadas ao gerenciamento e à operação de middleware orientado a mensagens, além
de permitir que os desenvolvedores se dediquem a criar diferenciais
O Amazon CloudWatch é um serviço de monitoramento e observação que fornece dados
e insights práticos para monitorar aplicativos, responder às alterações de performance
em todo o sistema, otimizar a utilização de recursos e obter uma visualização unificada
da integridade operacional. O CloudWatch coleta dados de monitoramento e operações
na forma de logs, métricas e eventos, oferecendo uma visualização unificada dos
recursos, dos aplicativos e dos serviços da AWS executados na AWS e em servidores
locais
O Amazon Simple Email Service (SES) é um serviço em nuvem de e-mail eficaz, flexível e
dimensionável. Com ele, os desenvolvedores podem enviar e-mails de qualquer
aplicação

#

## Pergunta 21: 
Sua empresa criou diversas funções Lambdas para consultar informações e compor
processos de avaliação de crédito. Qual serviço da AWS, orientado a eventos, pode ser
utilizado com pouca codificação para expressar lógicas de negócios complexas na forma
de fluxos de trabalho para construir esses processos?

- [ ] AWS SNS
- [X] AWS Step Functions
- [ ] AWS SQS
- [ ] AWS BPM

### Explicação

**Correta**

AWS Step Functions tem a finalidade de orquestrar todas as funções e também oferece a
visualização da execução do processo
https://aws.amazon.com/pt/step-functions/?nc2=h_ql_prod_ap_stf&step-
functions.sort-by=item.additionalFields.postDateTime&step-functions.sort-order=desc

**Incorretas**

O AWS BPM não é um serviço disponível na AWS.
O AWS SQS - Simple Queue Service é um serviço de mensageria recomendado pra
desacoplar sistemas e pode ser utilizado na arquitetura com Step Functions também.
O AWS SNS - Simple Message Service é um serviço de troca de mensagens
recomendado para arquiteturas Pub/Sub e utilização de tópicos e também pode ser
utilizado na arquitetura junto com o Step Function.

#

## Pergunta 22: 
Qual recurso da AWS habilita o usuário a gerenciar os serviços através de interface web?

- [ ] AWS Mobile First
- [X] AWS Management Console
- [ ] AWS Software Development Kit (SDK)
- [ ] AWS CloudWatch

### Explicação

**Correta**

AWS Console
https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/learn-whats-new.html

**Incorretas**

AWS Mobile First não é um serviço existente na AWS
AWS SDK fornece diversas bibliotecas para integração a IDE de diversas linguagens de
programação integrando com mais facilidade o desenvolvedor com os serviços da AWS.
Ex. Java, C#, Node, Python, entre outras
AWS CloudWatch serve para monitorar e gravar log de diversos serviços da AWS e de
aplicações desenvolvidas pelos clientes.

#

## Pergunta 23: Correto
Qual é a opção abaixo que faz uso da infraestrutura das Redes de Borda (EdgeLocations)
e Pontos de Presença para transferir em alta velocidade arquivos entre S3 Buckets?

- [ ] AWS DataSync
- [X] S3 Transfer Accelerations
- [ ] AWS VPN
- [ ] CloudFront

### Explicação

**Correta**

O Amazon S3 Transfer Acceleration é um recurso em nível de bucket que possibilita
transferências de arquivos rápidas, fáceis e seguras em longas distâncias entre o seu
cliente e um bucket do S3. O Transfer Acceleration tira proveito dos pontos de presença
distribuídos globalmente no Amazon CloudFront. Conforme os dados chegam em um
ponto de presença, eles são roteados para o Amazon S3 por um caminho de rede
otimizado.
https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/transfer-
acceleration.html

**Incorretas**

O CloudFront faz uso das redes de borda para cache de conteúdo.
O AWS DataSync tem a finalidade de transferir dados do ambiente on premise para a
AWS de forma automatizada.
O AWS VPN tem a finalidade de conectar redes com a AWS.

#

## Pergunta 24: 
Qual não é uma característica do Amazon Cognito?

- [ ] integra com a autenticação de mídias sociais como Apple, Facebook, Google e Amazon
- [ ] adiciona autenticação em aplicativo web e móveis
- [X] permite autenticação de APIS pela linha de comando
- [ ] integra com SAML 2.0 e OpenlD

### Explicação

**Correta**

O Amazon Cognito fornece autenticação, autorização e gerenciamento de usuários para
suas aplicações Web e móveis. Seus usuários podem fazer login diretamente com um
nome de usuário e uma senha ou por meio de terceiros, como o Facebook, a Amazon, o
Google ou a Apple.
Permite login social com Facebook, Google, Login with Amazon e Iniciar sessão com a
Apple, bem como por meio de provedores de identidade SAML e OIDC a partir do seu
grupo de usuários.
https://docs.aws.amazon.com/pt_br/cognito/latest/developerguide/what-is-amazon-
cognito.html

**Incorretas**

Permite autenticação de APIS pela linha de comando. O Cognito é um serviço indicado
para uso em aplicação, não em interações com serviços da AWS pela Linha de Comando.

#

## Pergunta 26: 

Qual é a melhor opção para salvar arquivos com pouca necessidade de uso?

- [ ] DynamoDb
- [X] S3 Glacier
- [ ] EC2
- [ ] S3 Standard

### Explicação

**Correta**

https://aws.amazon.com/s3/glacier/
S3 Glacier tem o custo otimizado, porém tem questões aos tempos de recuperação que
precisam ser considerados em qualquer implementação

**Incorretas**

O EC2 - Elastic Computing Cloud oferece é o serviço que oferece diversas configurações
de processamento e memória para alocar uma aplicação, não para armazenamento de
dados
O DynamoDb é um serviço de banco de dados não relacional para persistir os dados de
uma aplicação
O S3 - Simple Storage Service Standard é utilizado para salvar arquivos que sejam
acessados com frequência numa solução, o seu custo é mais alto por isso.

#

## Pergunta 27: 

A AWS é uma infraestrutura cloud global segura, extensível e confiável e que oferece
mais de 200 serviços em diversos países ao redor do mundo. Sobre sua distribuição no
mundo, podemos afirmar que?

- [ ] É atualmente composta por 6 regiões, que estão divididas em mínimo em 200 zonas de disponibilidade
- [ ] É atualmente composta por 6 zonas de disponibilidades(az) que estão divididas em mínimo em 200 regiões
- [ ] É atualmente composta por 31 zonas de disponibilidades(az), que estão divididas em aproximadamente 99 regiões de disponibilidade
- [X] É atualmente composta por 31 regiões, que estão divididas em aproximadamente 99 zonas de disponibilidade(az)

### Explicação

**Correta**

É composta por 29 regiões, que estão divididas em aproximadamente 93 zonas de
disponibilidade(az).
Essa informação pode mudar na medida que a AWS cresce e implementa data centers
em novos países.
https://aws.amazon.com/about-aws/global-infrastructure/?nc2=h_ql_le_int_gi

**Incorretas**

E atualmente composta por 29 zonas de disponibilidades(az), que estão divididas no
mínimo em 93 regiões de disponibilidade
O número de regiões é menor do que de zonas de disponibilidades, uma vez que uma
região pode conter 3 ou mais zonas de disponibilidade, cada uma com o seu
agrupamento de data centers.
E atualmente composta por 6 regiões, que estão divididas em mínimo em 200 zonas de
disponibilidade.
É atualmente composta por 6 zonas de disponibilidades(az) que estão divididas em
mínimo em 200 regiões
As regiões são posições estratégicas e não estão relacionadas a quantidade de
continentes ou países.

#

## Pergunta 28: 

Qual serviço oferece um grupo de ferramentas que podem ser usadas em conjunto ou
individualmente para permitir que desenvolvedores de front-end da web e de
dispositivos móveis criem aplicações seguras e escaláveis full-stack, com tecnologia
desenvolvida pela AWS?

- [ ] AWS Fargate
- [ ] AWS SDK
- [ ] AWS BeanStalk
- [X] AWS Amplify

### Explicação

**Correta**

O Amplify é um conjunto de ferramentas e recursos que permite que desenvolvedores
frontend desenvolvam para plataformas móveis e Web criem aplicações completas de
forma rápida e fácil na AWS. Eles podem contar com a flexibilidade do uso de todos os
serviços da AWS para se adaptar à evolução dos casos de uso. Com o Amplify, você pode
configurar o backend de uma aplicação Web ou móvel e conectá-la em minutos, criar
visualmente o frontend de uma IU para a Web e gerenciar facilmente o conteúdo da
aplicação fora do Console AWS
https://aws.amazon.com/pt/amplify/

**Incorretas**

O AWS Elastic Beanstalk é um serviço de fácil utilização para implantação e
escalabilidade de aplicações e serviços da web desenvolvidos com Java, .NET, PHP,
Node.js, Python, Ruby, Go e Docker em servidores familiares como Apache, Nginx,
Passenger e IIS.
AWS SDK permite que acesse e gerencie serviços da AWS com sua linguagem ou
plataforma de desenvolvimento preferencial
O AWS Fargate é um mecanismo de computação sem servidor para contêineres que
funciona com o ECS e EKS

#

## Pergunta 29: 
Uma aplicação crítica utiliza de 5 a 10 instâncias EC2 para suportar a grande volumetria
de requisição e processamento. Pelos seus estudos, essa infraestrutura atenderá a
necessidade pelos próximos 3 anos sem grandes alterações. Qual seria a melhor
estratégia para garantir a escalabilidade e otimizar os custos?

- [ ] 5 instâncias Reserved e 5 instâncias Spot
- [ ] 10 instâncias OnDemand
- [ ] 10 instâncias Reserved
- [X] 5 instâncias Reserved e 5 instâncias OnDemand

### Explicação

Como você já tem certeza que vai utilizar no mínimo 5 recursos é melhor ter desconto no
plano reserved (72% em relação ao onDemand) e manter as demais no plano onDemand
para usar de acordo com a necessidade pagando um pouco mais ou não pagando nada
se não precisar escalar.

#

## Pergunta 30: 
Qual é o serviço de DNS da AWS que, entre outras coisas, transforma nomes de urls em
código IP para acessar os recursos da Cloud?

- [ ] ELB
- [ ] ACL
- [ ] AWS Auto Scaling
- [X] Route53

### Explicação

**Correta**

O Amazon Route 53 é um serviço da Web de Sistema de Nomes de Domínio (DNS)
altamente disponível e escalável. O Route 53 conecta as requisições do usuário a
aplicações da Internet executadas na AWS ou on-premises,
https://aws.amazon.com/route53/?nc2=h_ql_prod_nt_r53

**Incorretas**

O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações
entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP,
funções do Lambda e dispositivos virtuais.
O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade
para manter um desempenho constante e previsível pelo menor custo possível.
ACL é uma camada opcional de segurança que você pode configurar como um firewall
para a sua Virtual Private Cloud

#

## Pergunta 31: 
Qual plano de suporte oferece um gerente técnico de conta para monitorar o ambiente
proativamente e sugerir melhorias para otimização dos serviços?

- [ ] Basic
- [ ] Developer
- [ ] Business
- [X] Enterprise

### Explicação

**Correta**

Apenas o plano de suporte enterprise oferece o gerenciamento de contas técnico.
Existem várias configurações de serviços de acordo com cada plano de suporte.
Os planos vigentes são Basic, Developer, Business, Enterprise on ramp e Enterprise.
As características que variam em cada plano são as seguintes:
- Verificação de práticas recomendas do AWS Trusted Advisor
- Suporte técnico aprimorado
- Tempo de resposta
- Orientações de arquitetura
- Gerenciamento programático de casos
- Suporte a software de terceiros
- Programas proativos e autoatendimento
- Gerenciamento de contas técnico
- Treinamento
- Assistência à conta
- Preço
https://aws.amazon.com/premiumsupport/plans/

**Incorretas**

Os outros planos das opções não oferecem esse serviço.
O plano enterprise on ramp, que foi lançado recentemente, oferece um grupo de
gerentes de contas técnicos para fornecer orientação proativa e coordenar o acesso a
programas e especialistas da AWS para o gerenciamento de contas técnico.

#

## Pergunta 32: 
Qual dos serviços abaixo é umas das formas de criar e gerenciar chaves de criptografia
para muitos serviços dentro da AWS?

- [ ] AWS Keys
- [ ] AWS KSM
- [ ] AWS Config
- [X] AWS KMS

### Explicação

**Correta**

KMS - Key Management Service
https://aws.amazon.com/kms/?nc2=type_a

**Incorretas**

O AWS Config é um serviço que permite acessar, auditar e avaliar as configurações dos
recursos da AWS. O Config monitora e grava continuamente registros das configurações
de recursos da AWS e lhe permite automatizar a avaliação das configurações registradas
com base nas configurações desejadas
AWS KSM e AWS Keys não existem

#

## Pergunta 33: Correto
Oual serviço da AWS é recomendado na implementação e no gerenciamento de banco
de dados relacionais?

- [X] RDS
- [ ] DMS
- [ ] DynamoDB
- [ ] KMS

### Explicação

**Correta**

O Amazon Relational Database Service (RDS) é uma coleção de serviços gerenciados
que facilita a configuração, operação e escalabilidade de bancos de dados na nuvem.
Oferta os mecanismos abaixo:
Amazon Aurora compatível com MySQL, Amazon Aurora compatível com PostgreSQL,
MySQL, MariaDB, PostgreSQL, Oracle e SQL Server. Depois, implante on-premises com
o Amazon RDS on AWS Outposts.
https:Waws.amazon.com/pt/rds/?nc2=type_a

**Incorretas**

O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados
para a AWS de modo rápido e seguro
O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves
criptográficas e o controle do seu uso em uma ampla variedade de serviços daAWS e em
seus aplicativos.
O Amazon DynamoDB é um banco de dados de valores-chave e documentos que oferece
desempenho em milissegundos de um dígito em qualquer escala. E um banco de dados
totalmente gerenciado, multirregional, multiativo e durável com segurança, backup e
restauração integrados e armazenamento em cache na memória para aplicativos em
escala de Internet

#

## Pergunta 34: 
Você vai lançar uma aplicação que precisa de 5 a 10 instâncias EC2 ativas de acordo com
a quantidade de usuários logados. Qual é o serviço da AWS que possui um mecanismo
para direcionar as requisições de forma distribuída entre esses servidores?

- [X] *ELB*
- [ ] Route53
- [ ] Securit Group
- [ ] Auto Scalling

### Explicação

**Correta**

ELB faz a distribuição de cargas entre as instâncias
https://aws.amazon.com/pt/elasticloadbalancing/?whats-new-cards-elb.sort-
by=item.additionalFields.postDateTime&whats-new-cards-elb.sort-order=desc

**Incorretas**

O Route53 é o DNS, servidor de domínios
O Security Group é a camada que protege o tráfego de dados de instâncias dentro de
uma rede ou subrede.
O Auto Scalling provisiona ou desprovisiona as instâncias necessárias para atender a
demanda dos usuários da aplicação.

#

## Pergunta 35: 
A migração dos serviços da sua empresa para a AWS vai precisar movimentar uma
quantidade muito grande de dados e a localização da sua infraestrutura atual não
permite que essa migração seja feita virtualmente devido a conectividade de rede muito
instável. Qual serviço da AWS oferece uma família de produtos para sua empresa
conseguir realizar essa migração de forma física?

- [ ] AWS DataSync
- [X] *AWS Snowball*
- [ ] AWS DirectConnect
- [ ] AWS DMS

### Explicação

**Correta**

AWS Snowball
Nestes casos de problemas com infraestrutura de datacenter e rede atuais, a AWS
fornece serviços que transportam seus dados em cases em caminhões, navios, aviões,
etc.. até a AWS.
https://aws.amazon.com/pt/snow/?nc2=h_ql_prod_mt_sno

**Incorretas**

O AWS DataSync é um serviço utilizado para realizar a sincronização de dados de forma
automática da sua infraestrutura on premisse com a AWS e utiliza as conexões de rede
estabelecidas.
O DMS - DataBase Migration Service é utilizado para realizar a migração de banco de
dados.
O AWS Direct Connect é uma solução de serviço de nuvem que facilita o
estabelecimento de uma conexão de rede dedicada entre suas instalações e a AWS

#

## Pergunta 36: 
Qual é o serviço de data warehouse da Amazon utilizado pelas áreas de BI, que permite o
cruzamento de vários dados estruturado e semi estruturados para gerar conhecimento
para o negócio?

- [X] *Amazon RedShift*
- [ ] Kinesis
- [ ] O EMR
- [ ] Power BI

### Explicação

**Correta**

O serviço do Amazon Redshift gerencia todo o trabalho de configuração, operação e
escalabilidade de um data warehouse. Essas tarefas incluem capacidade de
provisionamento, monitoramento e backup do cluster e aplicação de patches e
atualizações ao mecanismo Amazon Redshift.
https://docs.aws.amazon.com/pt_br/redshift/latest/mgmt/overview.html

**Incorretas**

O EMR é a plataforma de Big Data da AWS
O Power BI não é um serviço da AWS
O Kinesis é um serviço para transferir dados entre vários serviços da AWS através de
streaming

#

## Pergunta 37: 
Um dos 12 fatores para aplicações web em cloud é manter o cache de sessões de estado
do usuário em memória fora das instâncias EC2. Qual serviço abaixo é mais
recomendado para essa finalidade?

- [ ] Amazon S3
- [ ] Amazon EventBridge
- [X] Amazon ElasticCache for Redis
- [ ] Amazon EBS

### Explicação

**Correta**

ElasticCache for Redis
https://aws.amazon.com/pt/elasticache/redis/

**Incorretas**

O EBS fornece block storage para as instâncias EC2.
O S3 é o serviço de armazenamento padrão de objetos(arquivos + metadados) da AWS.
O EventBridge é um barramento de eventos para diversos serviços e aplicações da AWS.

#

## Pergunta 38: 
Qual serviço de mensageria é utilizado para desacoplar sistemas, escalar microsserviços
e compor arquiteturas de computação sem servidor e sem perder nenhuma mensagem?

- [X] SQS
- [ ] SNS
- [ ] Lambda
- [ ] Fargate

### Explicação

**Correta**

O Amazon Simple aueue Service (SQS) é um serviço de filas de mensagens gerenciado
que permite o desacoplamento e a escalabilidade de microsserviços, sistemas
distribuídos e aplicações sem servidor. O SOS elimina a complexidade e a sobrecarga
associadas ao gerenciamento e à operação de middleware orientado a mensagens, além
de permitir que os desenvolvedores se dediquem a criar diferenciais.
https://aws.amazon.com/pt/sqs/

**Incorretas**

SNS - Simple Notification Service é o serviço de Pub/Sub
O Lambda é utilizado para a implementação de funções sem servidor
O Fargate é utilizado para o uso de container sem servidor

#

## Pergunta 39: 
Qual é o serviço que permite coletar e armazenar logs de recursos, aplicativos e serviços,
praticamente em tempo real, para diversas finalidades de processos e negócio?

CloudTrail
Logs
CloudLogs
*CloudWatch Logs*

### Explicação

**Correta**

Você pode usar o Amazon CloudWatch Logs para monitorar, armazenar e acessar seus
arquivos de log em suas instâncias do Amazon Elastic Compute Cloud (Amazon EC2), no
AWS CloudTraiI, no Route 53 ou em outras origens. O CloudWatch Logs permite
centralizar os logs de todos os sistemas, aplicações e produtos da AWS que você usa em
um único serviço altamente escalável. Você pode facilmente visualizá-los, pesquisá-los
por códigos de erro ou padrões específicos, filtrá-los com base em campos específicos
ou arquivá-los com segurança para análise futura:
https://docs.aws.amazon.com/pt_br/AmazonCIoudWatch/Iatest/Iogs/WhatIsCIoudWatc
hLogs.html

**Incorretas**

CloudLogs e Logs não serviços disponíveis na AWS.
O CloudTrail é utilizado para logar ações de usuários em APIS de serviços da AWS, muito
utilizado em auditorias de uso das contas.

#

## Pergunta 40: 
Sua aplicação precisa que os dados estejam estruturados e distribuídos em tabelas,
relacionadas por chaves, para atender um requisito de uma funcionalidade. Qual banco
de dados abaixo não é indicado para esse fim?

MariaDB
Aurora
O MySql
*DynamoDB*

### Explicação

**Correta**

O DynamoDB não é um banco relacional e não atende esses requisitos
https://aws.amazon.com/pt/search/?searchQuery=AWS+Dynamo Db

**Incorretas**

Os demais bancos são relacionais e podem ser utilizados para a finalidade da questão.

#

## Pergunta 41: 
Qual serviço da AWS abaixo deve ser utilizado para liberar acesso na conta para 3
desenvolvedores novos que chegaram no seu time?

S3
EC2
CloudFront
*IAM*

### Explicação

**Correta**

IAM é o serviço utilizado para gestão de acessos de pessoas e aplicações na AWS.

**Incorretas**

S3 é para armazenar objetos, arquivos e seus metadados em Buckets
CloudFront é pra auxiliar na distribuição de conteúdo, diminuindo taxa de transferência e
melhorando a experiência do usuário na ponta.
EC2 é pra fornecer processamento, vários opções de computação

#

## Pergunta 42: 
Qual dos seguintes componentes de rede pode ser usado para hospedar recursos EC2
na AWS?

AWS Autoscaling
AWS Trusted Advisor
AWS Elastic Load Balancer
*AWS VPC*

### Explicação

**Correta**

O Amazon Virtual Private Cloud (Amazon VPC) oferece controle total sobre seu ambiente
de redes virtual, incluindo posicionamento de recursos, conectividade e segurança.
Comece a usar configurando sua VPC no console de serviço AWS. Em seguida, adicione
recursos a ela, como instâncias do Amazon Elastic Compute Cloud (EC2) e Amazon
Relational Database Service (RDS). Por fim, defina como suas VPCs se comunicam entre
si, entre contas, zonas de disponibilidade (AZs) ou Regiões da AWS. No exemplo abaixo,
o tráfego de rede está sendo compartilhado entre duas VPCs em cada região
https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html

**Incorretas**

ELB - O Elastic Load Balancing distribui automaticamente o tráfego de entrada de
aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres,
endereços IP, funções do Lambda e dispositivos virtuais.
O Amazon EC2 Auto Scaling ajuda a manter a disponibilidade das aplicações e permite
adicionar ou remover instâncias do EC2 automaticamente de acordo com as condições
que você definir.
O AWS Trusted Advisor faz recomendações que ajudam você a seguir as melhores
práticas da AWS. O Trusted Advisor avalia a sua conta através de verificações. Essas
verificações identificam formas de otimizar sua infraestrutura da AWS, aumentar a
segurança e o desempenho, reduzir os custos gerais e monitorar as cotas do serviço

#

## Pergunta 43:
Tráfego de dados é um item bastante relevante quando falamos de custos na AWS. Qual
das opções abaixo apresenta o cenário onde o tráfego é livre de custos?

transferência de dados de saída entre serviços do mesmo continente.
transferência de dados de saída entre serviços entre todas as Regiões
transferência de dados de saída entre serviços dentro da mesma Região (Region)
O Todo tráfego é cobrado

### Explicação

**Correta**

Os dados transferidos entre serviços na mesma região não têm custo, desta forma, os
dados que saem não são cobrados.
Outro cenário de gratuidade é o de entrada de dados.

**Incorretas**

Nem todo tráfego é cobrado.
Tráfego de saída entre regiões é cobrado.
Um continente pode conter mais de uma região e neste caso será cobrado.

#

## Pergunta 44: 
Qual é o serviço da AWS que pode ser utilizado para sua equipe desenvolver, compilar e
implantar, rapidamente, aplicativos na AWS a partir de modelos, além de disponibilizar
uma interface de usuário que permite o gerenciamento das atividades de
desenvolvimento de projeto e de problemas com base no Jira Atlassian?

AWS Codecommit
AWS CodeBuild
AWS CodeDeploy
AWS CodeStar

### Explicação

**Correta**

O AWS CodeStar permite a integração de várias ferramentas de desenvolvimento, desde
IDES, esteiras de CI/CD e gerenciamento de projetos para auxiliar e acelerar a entrega
de software. Disponibiliza vários modelos em diversas linguagens de programação para
acelerar o desenvolvimento de aplicativos.
https://aws.amazon.com/pt/codestar/

**Incorretas**

AWS CodeBuild é utilizado para compilar e testar o aplicativo na esteira.
AWS CodeCommit é utilizado para fazer o gerenciamento de código fonte.
AWS CodeDeploy é utilizado para fazer a implantação do aplicativo.

#

## Pergunta 45: 
Qual é a maneira mais fácil de lançar rapidamente milhares de containers em uma ampla
variedade de opções de computação da AWS, usando o seu CI/CD e ferramentas de
automação de sua preferência?

Com o Amazon Lambda
Com o Amazon EC2
*Com o Amazon ECS*
Com o Amazon CodePipeline

### Explicação

**Correta**

Amazon ECS - https://aws.amazon.com/pt/ecs/?nc2=h_ql_prod_ct_ecs&whats-new-cards.sort-
by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc&ecs-
blogs.sort-by=item.additionalFields.createdDate&ecs-blogs.sort-order=desc

**Incorretas**

O Lambda é utilizado implementar funções sem servidor na AWS
O EC2 é utilizado para implementar diversos tipos de máquinas para diversos usos em
aplicações na AWS, é base para o ECS, mas deve ser gerenciado pelo mesmo para
habilitar o uso fácil de container na AWS. E possível fazer manualmente o processo de
container no EC2, mas sem o ECS é muito mais trabalhoso.
O AWS CodePipeline é utilizado para a implementação de uma esteira de
desenvolvimento na AWS.

#

## Pergunta 46: 
Qual é o serviço da AWS que permite que os desenvolvedores foquem apenas na
codificação, enquanto realiza automaticamente o provisionamento de toda a
infraestrutura para a aplicação ser executada, o balanceamento das cargas, a
implementação de monitoramento e a implantação. Além disso, esse serviço permite a
codificação em .Net, Java, PHP, Node.js, Python, Ruby e Go entre outras.

*AWS ElasticBeanStalk*
AWS ECS
AWS CodeDeploy
Fargate

### Explicação

**Correta**

O Elastic Beanstalk implanta aplicações da Web para que você possa se concentrar em
seus negócios. E um serviço para implementar e escalar aplicações e serviços da Web
enquanto você só precisa se preocupar com o desenvolvimento do seu código. Esse
serviço gerencia automaticamente a implantação, desde o provisionamento de
capacidade, balanceamento de carga e escalabilidade automática até o monitoramento
da integridade de aplicações.
https:Waws.amazon.com/elasticbeanstalk/?nc2=h_ql_prod_cp_ebs

**Incorretas**

O AWS CodeDeploy é um serviço totalmente gerenciado de implantação que automatiza
implantações de software em diversos serviços de computação como Amazon EC2, AWS
Fargate, AWS Lambda e servidores locais.
O AWS Fargate é um mecanismo de computação sem servidor para contêineres
O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado
de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente
aplicações conteinerizadas

#

## Pergunta 47: 
Sua empresa iniciou um piloto de uma aplicação e ainda não tem a dimensão de quantos
clientes irão utilizá-la. Essa aplicação precisa ter alta disponibilidade e o piloto tem
previsão de duração de três meses. Qual plano de pagamento é o mais indicado para
esse contexto?

O Spot
Reserved
*On-Demand*
Dedicated Hosts

### Explicação

**Correta**

Como o tempo de piloto é de 2 meses e não temos dimensão dos usuários e de quantas
instâncias de máquinas serão utilizadas, o plano On-Demand é o mais indicado.

**Incorretas**

Reserved é recomendado quando já existe uma previsão de uso de no mínimo 1 ano.
Spot é recomendado para processos que não requerem provisionamento imediato.
Dedicated Hosts é indicado quando você necessita de servidores físicos dedicados.

#

## Pergunta 48: 
Usuários que fazem uso final de aplicações em cloud sem se preocuparem em como
foram construídas e implementadas fazem uso de qual tipo de cloud?

laaS
BaaS
PaaS
*SaaS*

### Explicação

**Correta**

SaaS - Software como serviço, a aplicação já está pronta para uso. Ex. e-mails, drivers,
etc.
https://aws.amazon.com/what-is-cIoud-computing/?nc2=h_qI_Ie_int_cc

**Incorretas**

- IaaS - Infraestrutura com serviço.

- PaaS - Plataforma como serviço.

- BaaS - Backend como serviço.

#

## Pergunta 49: 
Qual é o plano de suporte que oferece tempo de resposta menor que 15 minutos para
caso de sistema essencial aos negócios inativo?

*Enteprise*
Developer
Todos
Business

### Explicação

Os planos de suporte são o Basic, Developer, Business, Enterprise on-ramp(novo) e
Enterprise
Para o Basic e Developer não há menção de tempo de resposta para sistema de
produção inativo, pois esse planos não são recomendados para cargas de produção.
Para o Business é menos de 1 horas
Para o Enterprise on-ramp é menos de 30 minutos
Para o Enterprise é menos de 15 minutos
Recomendo estudar e comparar as diferenças dos planos diretamente no site da AWS
https://aws.amazon.com/pt/premiumsupport/plans/?nc=sn&loc=l

#

## Pergunta 50: 
Qual serviço utiliza Inteligência Artificial e analisa dados gerados por eventos de diversos
serviços e armazenados no S3, evitando que atividades maliciosas sejam realizadas?

AWS Shield
AWS Malicious
AWS GuardDuty
AWS Macie

### Explicação

**Correta**

AWS GuardDuty utiliza Inteligência Artificial e analisa dados gerados por eventos de
diversos serviços e armazenados no S3, evitando que atividades maliciosas sejam
realizadas
https://aws.amazon.com/guardduty/?nc2=h_qI_prod_se_gd

**Incorretas**

O Amazon Macie é um serviço de segurança e privacidade de dados totalmente
gerenciado que usa machine learning e correspondência de padrões para descobrir e
proteger seus dados confidenciais na AWS. A medida que as organizações gerenciam
volumes crescentes de dados, identificar e proteger seus dados confidenciais em escala
pode se tornar cada vez mais complexo, caro e demorado.
O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço
distribuída) que protege os aplicativos executados na AWS. O AWS Shield oferece de
detecção e mitigações em linha automáticas e sempre ativas que minimizam o tempo de
inatividade e a latência dos aplicativos, fornecendo proteção contra DDoS sem
necessidade de envolver o AWS Support.
AWS Malicius não existe.

#

## Pergunta 51: 
A área de marketing da sua empresa está planejando fazer uma campanha que durará 12
meses, em vista disso, você foi avisado que haverá um aumento no número de clientes
no site e viu que será necessário subir mais 3 instâncias EC2 para atender a demanda
durante esse período. Oual tipo de instância terá um melhor custo nesse cenário?

Spot
Reserved
Dedicated Hosts
*On Demand*

### Explicação

**Correta**

Nestes cenários com previsão de tempo de uso e processamento, o uso de instâncias
reservadas gera uma economia de até 72% em comparação ao modelo sob demanda (on
demand)

**Incorretas**

Por padrão o Dedicated Hosts é cobrado no modelo sob demanda, mais caro comparado
ao Reserved.
On-demand é mais caro que o o Reserved, mas não exige um acordo de tempo.
Spot é mais barato, mas faz uso da capacidade excedente da nuvem e não garante o
provisionamento programado para atender a carga no período especificado.

#

## Pergunta 52: 

Você desenvolveu um sistema de workflow orientado a eventos e gostaria que uma
função sem servidor gravasse uma log num banco de dados ao término do processo.
Qual serviço é o mais indicado para essa finalidade?

SQS
SNS
SES
*Lambda*

### Explicação

**Correta**

O AWS Lambda é um serviço de computação sem servidor e orientado a eventos que
permite executar código para praticamente qualquer tipo de aplicação ou serviço de
backend sem provisionar ou gerenciar servidores.
https://docs.aws.amazon.com/pt_br/lambda/latest/dg/welcome.html

**Incorretas**

SQS é o serivço de mensageria indicado para desacoplar sistemas.
SNS é o serviço de notificação no modelo Pub/Sub e tópicos.
SES é o serviço para o envio de e-mails.

#

## Pergunta 53: 
Seu time de desenvolvimento percebeu que 30% das consultas feitas por uma
aplicação no banco de dados trazem sempre o mesmo resultado. Qual é o serviço da
AWS que pode ser implementado para manter esses resultados em cache reduzindo os
acessos aos bancos de dados?

*Amazon ElasticCache*
Amazon EC2
Amazon EBS
Amazon Cache

### Explicação

**Correta**
AWS ElastiCache - https:Waws.amazon.com/elasticache/?nc2=h_ql_prod_db_elc

**Incorretas**

O Amazon Elastic Block Store (EBS) é um serviço de armazenamento em bloco fácil de
usar e de alta performance, projetado para uso com o Amazon Elastic Compute Cloud
(EC2) para taxas de transferência e cargas de trabalho intensivas de transações em
qualquer escala.
O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza
capacidade computacional segura e redimensionável na nuvem.
Amazon Cache não é um serviço existente na AWS

#

## Pergunta 54: 
Qual é o serviço utilizado para integrar contas AWS?

*AWS Organizations*
AWS MFA
AWS CloudFormation
AWS Cost Explorer

### Explicação

**Correta**

O AWS Organization permite agrupar contas e também permite agrupa Organizations.
Dessa forma você pode ter Uma Organization com diversas Organizations, com diversas
contas, muito útil para empresas muito grandes.

**Incorretas**

AWS Cost Explorer para explorar custos que sua infraestrutura está consumindo
MFA - Fator de Autenticação duplo, que adiciona um passo a mais na autenticação do
acesso
CloudFormation - utilizado para IAC, Infraestrutura como código, onde são definidos
arquivos templates com todos os serviços e configurações que se deseja implementar
numa infraestrutura.

#

## Pergunta 55: 

Qual é a melhor definição para Region(Região)?

*Uma localização geográfica no mundo que agrupa algumas availability zones(zonas de disponibilidade) e edge locations(redes de borda).*
Uma region(região) é um data center dentro de uma avalibility zone(zonas de disponibilidade)
Uma region(região) é a mesma coisa que uma edge location(rede de borda)
Uma region(região) é um continente que aloca todos os data centers da AWS.

### Explicação

**Correta**

A Nuvem AWS abrange aproximadamente 93 zonas de disponibilidade em 29 regiões
geográficas em todo o mundo, mais de 400 locais da borda e 13 caches de borda
regionais.
Uma região pode abranger mais de 1 país e 1 país pode ter mais de 1 região, dependendo
da quantidade de clientes, localização, questões geopolíticas e estratégia de expansão
da AWS.
A região de São Paulo atualmente é composta por 3 zonas de disponibilidade, cada zona
de disponibilidade pode ser composta por um ou mais data centers agrupados e isolados
logicamente para garantir a alocação de serviços de forma redundante na mesma Região
e garantir a alta disponibilidade e resiliência das aplicações. Além disso, a Região pode
conter data centers em redes de borda próximos aos usuários para fazer cache de
conteúdo e melhorar a latência das aplicações. Esses data centers não podem ser
utilizados como zona de disponibilidade para a implementação direta como serviços
como o EC2 , RDS, etc, apenas são utilizados por serviços como o CloudFront ou
ApiGateway para fazer cache de arquivos e dados.

**Incorretas**

Região, zonas de disponibilidade e redes de borda são itens distintos na infraestrutura
global da AWS.
Um continente pode terl ou mais regiões da AWS. Atualmente na América do Norte
existem mais de 6, enquanto na América do Sul e na Africa existem 1.

#

## Pergunta 56: 
Qual dos pilares do Well-Architected Framework foca em como podemos continuamente
melhorar processos e procedimentos?

*Excelência Operacional*
Segurança
Confiabilidade
Performance Eficiente

### Explicação

**Correta**

O pilar Excelência operacional se concentra na execução e monitoramento sistemas e na
melhoria contínua de processos e procedimentos. Os principais tópicos incluem
automação de alterações, reação a eventos e definição de padrões para gerenciar as
operações diárias.
A AWS Well-Architected ajuda arquitetos de nuvem a construir infraestruturas seguras,
resilientes, eficientes e de alta performance para aplicações e workloads. Baseado em
seis pilares (excelência operacional, segurança, confiabilidade, eficiência de
performance, otimização de custos e sustentabilidade), o AWS Well-Architected fornece
uma abordagem consistente para que clientes e parceiros avaliem arquiteturas e
implementem designs que podem se expandir com o tempo.
https://aws.amazon.com/pt/architecture/well-architected/?wa-lens-whitepapers.sort-
by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc

**Incorretas**

O pilar Segurança se concentra na proteção de informações e sistemas.
O pilar da confiabilidade se concentra nos workloads que executam as funções
pretendidas e na recuperação rápida de falhas em atender demandas.
O pilar de eficiência de performance se concentra na alocação estruturada e simplificada
de recursos de Tl e computação.

#

## Pergunta 57: 
Qual é a classe de armazenamento do S3 que pode diminuir os custos, à medida que
move os objetos automaticamente entre camadas, de acordo com a frequência de uso?

S3 Standard
S3 Standard Infrequent Access
S3 Glacier
*S3 Intelligent-Tiering*

### Explicação

**Correta**

S3 Intelligent-Tiering
https:Waws.amazon.com/s3/storage-classes/?nc=sn&loc=3

**Incorretas**

As demais classes não fazem a movimentação automática para as demais camadas.

#

## Pergunta 58: 
Qual é o serviço de integração, totalmente gerenciado pela AWS, que permite transferir
dados com segurança entre aplicativos de Software como Serviço (SaaS) como:
Salesforce, Zendesk, Slack e ServiceNow, Amazon S3 e Amazon Redshift?

Amazon DMS
Amazon SNS
*Amazon AppFlow*
Amazon EventBridge

### Explicação

**Correta**

Com o AppFlow, você não precisa investir tempo significativo e uma equipe de
desenvolvedores altamente qualificada para criar e manter conectores de API
personalizados de serviços da AWS com o objetivo de fazer o intercâmbio de dados com
aplicativos de SaaS.
https:Waws.amazon.com/pt/appflow/?nc2=h_ql_prod_ap_af

**Incorretas**

O Amazon EventBridge é um barramento de eventos sem servidor que torna mais fácil a
criação de aplicações orientadas por eventos em escala usando eventos gerados com
base em suas aplicações, aplicações integradas de software como serviço (SaaS) e
serviços da AWS
O Amazon Simple Notification Service (Amazon SNS) é um serviço de mensagens
totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de
aplicação para pessoa (A2P).A funcionalidade pub/sub de A2A fornece tópicos para
sistemas de mensagens de alta taxa de transferência baseados em push e de muitos
para muitos entre sistemas distribuídos, microserviços e aplicativos sem servidor
orientados por eventos
O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados
para a AWS de modo rápido e seguro. O banco de dados de origem permanece
totalmente operacional durante a migração, minimizando o tempo de inatividade de
aplicações que dependem do banco de dados

#

## Pergunta 59: 
Você deseja disponibilizar sua aplicação no endereço www.simuladoudemy.com. Qual
serviço pode ser utilizada para essa finalidade?

API Gateway
AutoScalling
*Route 53*
S3

### Explicação

**Correta**

Se você deseja criar um site ou um aplicativo web, comece registrando o nome do seu
site, conhecido como nome de domínio. O seu nome de domínio é o nome, como
exemplo.com, que seus usuários inserem em um navegador para exibir o site, que pode
ser registrado e gerenciado pelo Route 53
https://docs.aws.amazon.com/pt_br/Route53/Iatest/DeveIoperGuide/WeIcome.htmI

**Incorretas**

O API Gateway é utilizado para o gerenciamento de APIs.
O Auto Scalling é utilizado para escalar automaticamente o número de instâncias
necessárias para suportar a carga necessária para executar as aplicações.
O S3 pode ser habilitado para hospedar um site estático através de uma url do serviço,
não por um domínio desejado pelo cliente.

#

## Pergunta 60: 
Qual é o serviço da AWS que permite selecionar uma imagem de uma máquina pré-
configurada para lançar uma instâncias EC2?

*AMI*
IAM
AWS IMG
Amazon Image

### Explicação

**Correta**

Uma Imagem de máquina da Amazon (AMI) fornece as informações necessárias para
iniciar uma instância. Você deve especificar uma AMI ao iniciar uma instância. Você pode
executar várias instâncias em uma única AMI quando precisa de várias instâncias com a
mesma configuração. Você pode usar AMIs diferentes para executar instâncias quando
precisa de instâncias com configurações diferentes.
https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/AM Is.html

**Incorretas**

O AWS Identity and Access Management (IAM) permite que você gerencie com
segurança o acesso aos serviços e recursos da AWS. Usando o IAM, você pode criar e
gerenciar usuários e grupos da AWS e usar permissões para conceder e negar acesso a
recursos da AWS.
Amazon Image e Amazon IMG não existem.

#

## Pergunta 61: Incorreto
Quais dos itens abaixo fazem parte dos pilares do Well-Architected Framework? (Selecione 4 alternativas)

*Performance Eficiente*
Agilidade
*Sustentabilidade*
*Otimização de Custos*
*Confiabilidade*

### Explicação

**Correta**s

Os pilares são Excelência Operacional, Segurança, Confiabilidade, Performance
Eficiente, Otimização de Custos e Sustentabilidade.
https://aws.amazon.com/architecture/well-architected/?nc2=h_ql_le_wa&wa-lens-
whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-
order=desc

#

## Pergunta 62: 
Um objeto de um Bucket do AWS S3 é composto por quais itens abaixo? (selecione 2)

Role
Arquivo
Metadados
Policy

### Explicação

**Correta**

Pode ser composto por arquivo e opcionalmente pelo Metadado do arquivo
https://aws.amazon.com/pt/s3/getting-started/?nc=sn&loc=6&dn=1

**Incorretas**

Role e Policy são recursos gerenciados pelo IAM.


#

## Pergunta 63: Correto
Quais são as principais funcionalidades do Amazon SageMaker? (selecione dois)

*Oferecer uma IDE para uso de Machine Learning*
Preparar, Construir e implantar APIs Rest
*Preparar, Construir, Treinar e Implantar modelos de machine learning na AWS*
Preparar, Construir e Implantar modelos de banco de dados na AWS
Preparar, documentar e publicar APIs com raml sawgger

### Explicação

O SageMaker é a plataforma com diversos serviços para apoia desenvolvedores e
cientista de dados na implementação de aprendizado de máquina na AWS (Machine
Learning)
Visão dos processos de ML
https://aws.amazon.com/pt/sagemaker/

#

## Pergunta 64: 
Qual dos seguintes serviços permite registros de novos domínios?

IAM
ELB
*Route53*
AWS DNS

### Explicação

**Correta**

Route53 - https:Waws.amazon.com/route53/?nc2=type_a

**Incorretas**

O AWS Identity and Access Management (IAM) permite que você gerencie com
segurança o acesso aos serviços e recursos da AWS. Usando o IAM, você pode criar e
gerenciar usuários e grupos da AWS e usar permissões para conceder e negar acesso a
recursos da AWS
O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações
entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP,
funções do Lambda e dispositivos virtuais.
AWS DNS não é um serviço existente na AWS

#

## Pergunta 65: 
Qual serviço da AWS faz recomendações para a otimização de segurança dos seus
recursos?

MFA
IAM
Security Group
*Trusted Advisor*

### Explicação

**Correta**

Trusted Advisor faz diversas recomendações de acordo com o plano de suporte
contratado. As recomendações de otimização de segurança são algumas delas.
https://aws.amazon.com/pt/premiumsupport/technology/trusted-advisor/

**Incorretas**

O IAM é utilizado para fazer o gerenciamento dos usuários, dos grupos e dos acessos as
aplicações
O MFA é utilizado para adicionar um passo a mais no processo de autenticação do
usuário no acesso a conta pela console.
O Security Group é uma camada de proteção utilizada para permitir ou negar o tráfego
de dados em uma ou mais instâncias dentro de uma rede privada vitual.
