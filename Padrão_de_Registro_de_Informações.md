**Padrão de Registro de Informações**

**Status da Última Atualização: Atualizado em outubro de 2022**

**Isenção de Uso Gratuito:** Esta política foi criada pelo SANS Institute para a comunidade da Internet. Você pode usar toda ou parte desta política livremente em sua organização. Não é necessário aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um email para policy-resources@sans.org.

**1. Visão Geral**
A geração de registros (logs) de sistemas críticos, aplicativos e serviços pode fornecer informações importantes e potenciais indicadores de comprometimento. Embora as informações de registro possam não ser visualizadas diariamente, é fundamental tê-las do ponto de vista forense.

**2. Propósito**
O objetivo deste documento é abordar essa questão identificando requisitos específicos que os sistemas de informações devem atender para gerar registros de auditoria apropriados e integrar-se à função de gerenciamento de logs da empresa.

A intenção é que esta linguagem possa ser facilmente adaptada para uso em políticas e padrões de segurança de TI da empresa, bem como em padrões de aquisição de empresas e modelos de RFP. Dessa forma, as organizações podem garantir que os novos sistemas de TI, sejam desenvolvidos internamente ou adquiridos, suportem a geração e o gerenciamento de logs de auditoria necessários.

**3. Abrangência**
Esta política se aplica a todos os sistemas de produção na Rede <Nome da Empresa>.

**4. Política**

**4.1 Requisitos Gerais**
Todos os sistemas que lidam com informações confidenciais, aceitam conexões de rede ou tomam decisões de controle de acesso (autenticação e autorização) devem registrar e manter informações de registro de auditoria suficientes para responder às seguintes perguntas:
4.1.1 Que atividade foi realizada?
4.1.2 Quem ou o que realizou a atividade, incluindo onde ou em que sistema a atividade foi realizada (sujeito)?
4.1.3 Em que o que a atividade foi realizada (objeto)?
4.1.4 Quando a atividade foi realizada?
4.1.5 Com quais ferramentas a atividade foi realizada?
4.1.6 Qual foi o status (como sucesso versus falha), resultado ou resultado da atividade?

**4.2 Atividades a Serem Registradas**
Portanto, os registros devem ser criados sempre que uma das seguintes atividades for solicitada pelo sistema:
4.2.1 Criar, ler, atualizar ou excluir informações confidenciais, incluindo informações de autenticação confidenciais, como senhas;
4.2.2 Criar, atualizar ou excluir informações não abrangidas no item 1;
4.2.3 Iniciar uma conexão de rede;
4.2.4 Aceitar uma conexão de rede;
4.2.5 Autenticação e autorização do usuário para atividades abrangidas pelos itens 1 ou 2, como login e logout de usuário;
4.2.6 Conceder, modificar ou revogar direitos de acesso, incluindo adicionar um novo usuário ou grupo, alterar os níveis de privilégio do usuário, alterar permissões de arquivo, alterar permissões de objeto de banco de dados, alterar regras de firewall e alterações de senha do usuário;
4.2.7 Mudanças na configuração de sistemas, rede ou serviços, incluindo instalação de patches e atualizações de software ou outras alterações de software instalado;
4.2.8 Inicialização, desligamento ou reinicialização de processos de aplicativo;
4.2.9 Aborto, falha ou término anormal de processos de aplicativo, especialmente devido à exaustão de recursos ou ao atingimento de um limite ou limiar de recursos (como para CPU, memória, conexões de rede, largura de banda de rede, espaço em disco ou outros recursos), falha de serviços de rede, como DHCP ou DNS, ou falha de hardware; e
4.2.10 Detecção de atividade suspeita/maliciosa, como de um Sistema de Detecção ou Prevenção de Intrusões (IDS/IPS), sistema antivírus ou sistema anti-spyware.

**4.3 Elementos do Registro**
Tais registros devem identificar ou conter pelo menos os seguintes elementos, direta ou indiretamente. Nesse contexto, o termo "indiretamente" significa inferido de forma incontestável.
4.3.1 Tipo de ação - exemplos incluem autorizar, criar, ler, atualizar, excluir e aceitar conexão de rede.
4.3.2 Subsistema que realiza a ação - exemplos incluem nome do processo ou transação, identificador do processo ou transação.
4.3.4 Identificadores (quantos estiverem disponíveis) para o sujeito que solicitou a ação - exemplos incluem nome de usuário, nome do computador, endereço IP e endereço MAC. Observa-se que esses identificadores devem ser padronizados para facilitar a correlação de registros.
4.3.5 Identificadores (quantos estiverem disponíveis) para o objeto sobre o qual a ação foi realizada - exemplos incluem nomes de arquivo acessados, identificadores exclusivos de registros acessados em um banco de dados, parâmetros de consulta usados para determinar registros acessados em um banco de dados, nome do computador, endereço IP e endereço MAC. Observa-se que esses identificadores devem ser padronizados para facilitar a correlação de registros.
4.3.6 Valores antes e depois quando a ação envolve a atualização de um elemento de dados, se for viável.
4.3.7 Data e hora em que a ação foi realizada, incluindo informações relevantes de fuso horário, se não estiver no Tempo Universal Coordenado (Coordinated Universal Time - UTC).
4.3.8 Se a ação foi permitida ou negada pelos mecanismos de controle de acesso.
Descrição e/ou códigos de motivo de por que a ação foi negada pelo mecanismo de controle de acesso, se aplicável.

**4.4 Formato e Armazenamento**
O sistema deve suportar o formato e o armazenamento de registros de auditoria de tal forma a garantir a integridade dos registros e a apoiar a análise e a geração de relatórios em nível corporativo. Observa-se que a construção de um mecanismo real de gerenciamento de logs em nível

 corporativo está fora do escopo deste documento. Mecanismos conhecidos que suportam esses objetivos incluem, mas não se limitam aos seguintes:
4.4.1 Registros de Eventos do Microsoft Windows coletados por um sistema de gerenciamento de logs centralizado;
4.4.2 Registros em um formato bem documentado enviados via protocolos de rede syslog, syslog-ng ou syslog confiáveis para um sistema de gerenciamento de logs centralizado;
4.4.3 Registros armazenados em um banco de dados ANSI-SQL que gera registros de auditoria em conformidade com os requisitos deste documento; e
4.4.4 Outros mecanismos de registro abertos que suportam os requisitos acima, incluindo aqueles baseados em CheckPoint OpSec, ArcSight CEF e IDMEF.

**5. Conformidade com a Política**

**5.1 Medição da Conformidade**
A equipe de Infosec verificará a conformidade com esta política por meio de diversos métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.

**5.2 Exceções**
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Infosec.

**5.3 Não Conformidade**
Um funcionário que violar esta política pode estar sujeito a ações disciplinares, incluindo a rescisão do emprego.

**6. Normas, Políticas e Processos Relacionados**
Nenhum.

**7. Definições e Termos**
Nenhum.

**8. Histórico de Revisões**

**Data da Alteração** **Responsável** **Sumário da Alteração**
Junho de 2014 **Equipe de Políticas SANS** **Atualizado e convertido para novo formato.**
Outubro de 2022 **Equipe de Políticas SANS** **Convertido para novo formato.**
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.