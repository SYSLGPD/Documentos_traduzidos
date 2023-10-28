# Política de Segurança para Laboratórios

**Última Atualização:** Atualizado em outubro de 2022

**Aviso de Uso Livre:** Esta política foi criada pelo SANS Institute para a comunidade da Internet. Todo ou parte deste documento pode ser livremente usado em sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou versão atualizada, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

Consulte o Propósito.

## 2. Propósito

Esta política estabelece os requisitos de segurança da informação para ajudar a gerenciar e proteger os recursos de laboratórios e redes da <Nome da Empresa> minimizando a exposição da infraestrutura crítica e ativos de informação a ameaças resultantes de hosts desprotegidos e acesso não autorizado.

## 3. Abrangência

Esta política se aplica a todos os funcionários, contratados, consultores, trabalhadores temporários e outros na <Nome da Empresa> e suas subsidiárias que devem obedecer a esta política. Esta política se aplica aos laboratórios de propriedade e gerenciados pela <Nome da Empresa>, incluindo laboratórios fora do firewall corporativo (DMZ).

## 4. Política

### 4.1 Requisitos Gerais

#### 4.1.1 Organizações proprietárias de laboratórios são responsáveis por designar gerentes de laboratório, um ponto de contato (POC) e um POC alternativo para cada laboratório. Os proprietários de laboratórios devem manter as informações atualizadas do POC com o InfoSec e a equipe de Gerenciamento Corporativo. Os gerentes de laboratório ou seus substitutos devem estar disponíveis 24 horas por dia para emergências; caso contrário, as ações serão tomadas sem a participação deles.

#### 4.1.2 Os gerentes de laboratório são responsáveis pela segurança de seus laboratórios e pelo impacto do laboratório na rede de produção corporativa e em outras redes. Os gerentes de laboratório são responsáveis por aderir a esta política e aos processos associados. Onde políticas e procedimentos não estiverem definidos, os gerentes de laboratório devem fazer o melhor para proteger a <Nome da Empresa> contra vulnerabilidades de segurança.

#### 4.1.3 Os gerentes de laboratório são responsáveis pela conformidade do laboratório com todas as políticas de segurança da <Nome da Empresa>.

#### 4.1.4 O Gerente de Laboratório é responsável por controlar o acesso ao laboratório. O acesso a qualquer laboratório específico será concedido apenas pelo gerente de laboratório ou por um representante designado, a indivíduos com uma necessidade de negócios imediata dentro do laboratório, seja de curto prazo ou conforme definido por sua função de trabalho em curso. Isso inclui a monitorização contínua da lista de acesso para garantir que aqueles que não necessitam mais de acesso ao laboratório tenham seu acesso encerrado.

#### 4.1.5 Todas as senhas de usuário devem estar em conformidade com a Política de Senhas da <Nome da Empresa>.

#### 4.1.6 Contas de usuário individuais em qualquer dispositivo de laboratório devem ser excluídas quando não estiverem mais autorizadas, no prazo de três (3) dias. Senhas de contas de grupo em computadores de laboratório (Unix, Windows, etc.) devem ser alteradas trimestralmente (a cada 3 meses).

#### 4.1.7 Computadores de laboratório baseados em PC devem ter o software antivírus padrão e suportado pela <Nome da Empresa> instalado e programado para ser executado em intervalos regulares. Além disso, o software antivírus e os arquivos de padrões de vírus devem ser mantidos atualizados. Computadores infectados por vírus devem ser removidos da rede até serem verificados como livres de vírus. Os Administradores de Laboratórios/Gerentes de Laboratório são responsáveis por criar procedimentos que garantam que o software antivírus seja executado em intervalos regulares e que os computadores sejam verificados como livres de vírus.

#### 4.1.8 Qualquer atividade com a intenção de criar e/ou distribuir programas maliciosos nas redes da <Nome da Empresa> (por exemplo, vírus, worms, cavalos de Troia, bombas de e-mail, etc.) é proibida, de acordo com a Política de Uso Aceitável.

#### 4.1.9 Nenhum laboratório deverá fornecer serviços de produção. Serviços de produção são definidos como serviços críticos de negócios contínuos e compartilhados que geram receitas ou fornecem capacidades ao cliente. Esses serviços devem ser gerenciados por uma organização de suporte apropriada.

#### 4.1.10 De acordo com a Política de Classificação de Dados, informações marcadas como Altamente Confidenciais da <Nome da Empresa> ou Restritas da <Nome da Empresa> são proibidas nos equipamentos de laboratório.

#### 4.1.11 Acesso imediato aos registros de equipamento e sistema deve ser concedido aos membros do InfoSec e da Organização de Suporte de Rede, mediante solicitação, de acordo com a Política de Auditoria.

#### 4.1.12 O InfoSec analisará solicitações de renúncia à não conformidade caso a caso e aprovará renúncias, se justificado.

### 4.2 Requisitos Internos de Segurança do Laboratório

#### 4.2.1 A Organização de Suporte de Rede deve manter um dispositivo de firewall entre a rede de produção corporativa e todos os equipamentos de laboratório.

#### 4.2.2 A Organização de Suporte de Rede e/ou o InfoSec reservam o direito de interromper conexões de laboratório que afetem negativamente a rede de produção corporativa ou representem um risco de segurança.

#### 4.2.3 A Organização de Suporte de Rede deve registrar todos os endereços IP do laboratório que são roteados nas redes da <Nome da Empresa>, juntamente com informações de contato atualizadas para esse laboratório.

#### 4.2.4 Qualquer laboratório que deseje adicionar uma conexão externa deve fornecer um diagrama e documentação ao InfoSec com justificativa comercial, informações de equipamento e espaço de endereço IP. O InfoSec revisará em busca de preocupações de

 segurança e deve aprovar antes que tais conexões sejam implementadas.

#### 4.2.5 Todo o tráfego entre a rede de produção corporativa e a rede de laboratório deve passar por um firewall mantido pela Organização de Suporte de Rede. Os dispositivos de rede de laboratório (incluindo sem fio) não devem interconectar as redes de laboratório e de produção.

#### 4.2.6 As configurações originais do firewall e quaisquer alterações subsequentes devem ser revisadas e aprovadas pelo InfoSec. O InfoSec pode exigir melhorias de segurança conforme necessário.

#### 4.2.7 Os laboratórios são proibidos de realizar varreduras de portas, descoberta automática de rede, envio/geração de tráfego e outras atividades semelhantes que afetem negativamente a rede corporativa e/ou redes não pertencentes à <Nome da Empresa>. Essas atividades devem ser restritas dentro do laboratório.

#### 4.2.8 O tráfego entre as redes de produção e de laboratório, bem como o tráfego entre redes de laboratório separadas, é permitido com base em necessidades comerciais, desde que o tráfego não afete negativamente outras redes. Os laboratórios não devem anunciar serviços de rede que possam comprometer serviços de rede de produção ou expor informações confidenciais do laboratório.

#### 4.2.9 O InfoSec reserva o direito de auditar todos os dados relacionados a laboratórios e processos administrativos a qualquer momento, incluindo, mas não se limitando a, pacotes de entrada e saída, firewalls e periféricos de rede.

#### 4.2.10 Dispositivos de gateway de propriedade do laboratório devem estar em conformidade com todos os avisos de segurança de produtos da <Nome da Empresa> e devem se autenticar nos servidores de autenticação corporativa.

#### 4.2.11 A senha de habilitação para todos os dispositivos de gateway de laboratório deve ser diferente das senhas de outros equipamentos no laboratório. A senha deve estar de acordo com a Política de Senhas da <Nome da Empresa>. A senha só será fornecida a pessoas autorizadas a administrar a rede do laboratório.

#### 4.2.12 Em laboratórios onde pessoas não pertencentes à <Nome da Empresa> têm acesso físico (por exemplo, laboratórios de treinamento), a conectividade direta à rede de produção corporativa não é permitida. Além disso, nenhuma informação confidencial da <Nome da Empresa> pode residir em nenhum equipamento de computação nesses laboratórios. A conectividade para pessoal autorizado desses laboratórios pode ser permitida na rede de produção corporativa somente se for autenticada nos servidores de autenticação corporativa, listas de acesso temporárias (chave e fechadura), SSH, VPNs de cliente ou tecnologia semelhante aprovada pelo InfoSec.

#### 4.2.13 Laboratórios com conexões externas não podem se conectar à rede de produção corporativa ou a outras redes internas através de uma conexão direta, conexão sem fio ou equipamento de computação.

### 4.3 Requisitos de Segurança do Laboratório DMZ

#### 4.3.1 Novos laboratórios DMZ exigem uma justificação comercial e aprovação em nível de VP da unidade de negócios. Mudanças na conectividade ou finalidade de um laboratório DMZ existente devem ser revisadas e aprovadas pela equipe do InfoSec.

#### 4.3.2 Laboratórios DMZ devem estar em uma sala separada fisicamente, gaiola ou rack fechado com acesso limitado. Além disso, o Gerente de Laboratório deve manter uma lista das pessoas que têm acesso ao equipamento.

#### 4.3.3 Os POCs dos laboratórios DMZ devem manter os dispositivos de rede implantados no laboratório DMZ até o ponto de demarcação da organização de suporte de rede.

#### 4.3.4 Os laboratórios DMZ não podem se conectar às redes internas da empresa, seja diretamente, logicamente (por exemplo, túnel IPSEC), por meio de uma conexão sem fio ou de uma máquina multirreferência.

#### 4.3.5 Uma organização de suporte de rede aprovada deve manter um dispositivo de firewall entre o laboratório DMZ e a Internet. Dispositivos de firewall devem ser configurados com base nos princípios de acesso com privilégios mínimos e nos requisitos de negócios do laboratório DMZ. Configurações originais de firewall e alterações subsequentes devem ser revisadas e aprovadas pela equipe do InfoSec. Todo o tráfego entre o laboratório DMZ e a Internet deve passar pelo firewall aprovado. Conexões cruzadas que contornem o dispositivo de firewall são estritamente proibidas.

#### 4.3.6 Todos os roteadores e switches que não são usados para testes e/ou treinamento devem estar em conformidade com os documentos de padronização de roteadores e switches do DMZ.

#### 4.3.7 Os sistemas operacionais de todos os hosts internos ao laboratório DMZ que executam serviços de Internet devem ser configurados de acordo com os padrões de instalação e configuração segura publicados pela equipe do InfoSec.

#### 4.3.8 A administração remota deve ser realizada por canais seguros (por exemplo, conexões de rede criptografadas usando SSH ou IPSEC) ou acesso à console independente das redes do laboratório DMZ.

#### 4.3.9 Os dispositivos do laboratório DMZ não devem ser um proxy aberto para a Internet.

#### 4.3.10 A organização de suporte de rede e o InfoSec reservam o direito de interromper conexões de laboratório se houver preocupação de segurança.

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade
A equipe de InfoSec verificará a conformidade com esta política por meio de vários métodos, incluindo, entre outros, relatórios de ferramentas de negócios, auditorias internas e externas e feedback para o proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de InfoSec.

## 5.3 Não Conformidade

Um funcionário que for encontrado em violação desta política poderá estar sujeito a ações disciplinares, incluindo demissão.

## 6. Normas, Políticas e Processos Relacionados

- Política de Auditoria
- Política de Uso Aceitável
- Política de Classificação de Dados
- Política de Senhas

## 7. Definições e Termos

As seguintes definições e termos podem ser encontrados no Glossário da SANS localizado em: [https://www.sans.org/security-resources/glossary-of-terms/](https://www.sans.org/security-resources/glossary-of-terms/)

- DMZ (Zona Desmilitarizada)
- Firewall (Firewall)

## 8. Histórico de Revisão

Data da Mudança | Responsável | Resumo da Mudança
--- | --- | ---
Junho de 2014 | Equipe de Políticas da SANS | Atualizado, tornou o laboratório geral e incluiu requisitos de laboratório de DMZ, e converteu para novo formato.
Outubro de 2022 | Equipe de Políticas da SANS | Convertido para novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.