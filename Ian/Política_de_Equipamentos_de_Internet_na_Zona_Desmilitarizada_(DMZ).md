**Política de Equipamentos de Internet na Zona Desmilitarizada (DMZ)**

**Status da Última Atualização: Retirada**

**Isenção de Uso Gratuito:** Esta política foi criada pelo SANS Institute para a comunidade da Internet. Você pode usar toda ou parte desta política livremente em sua organização. Não é necessário aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um email para policy-resources@sans.org.

**1. Visão Geral**
Consulte o Propósito.

**2. Propósito**
O propósito desta política é definir padrões a serem atendidos por todos os equipamentos de propriedade e/ou operados pela <Nome da Empresa> localizados fora dos firewalls corporativos da <Nome da Empresa>. Esses padrões são projetados para minimizar a exposição potencial da <Nome da Empresa> à perda de dados confidenciais ou sigilosos, propriedade intelectual, danos à imagem pública, etc., que podem resultar do uso não autorizado dos recursos da <Nome da Empresa>.

Dispositivos que estão expostos à Internet e fora do firewall da <Nome da Empresa> são considerados parte da "zona desmilitarizada" (DMZ) e estão sujeitos a esta política. Esses dispositivos (rede e host) são particularmente vulneráveis a ataques da Internet, uma vez que residem fora dos firewalls corporativos.

A política define os seguintes padrões:
•	Responsabilidade de propriedade
•	Requisitos de configuração segura
•	Requisitos operacionais
•	Requisito de controle de mudanças

**3. Abrangência**
Todos os equipamentos ou dispositivos implantados em uma DMZ de propriedade e/ou operados pela <Nome da Empresa> (incluindo hosts, roteadores, switches, etc.) e/ou registrados em qualquer domínio do Sistema de Nomes de Domínio (DNS) de propriedade da <Nome da Empresa> devem seguir esta política.

Esta política também abrange qualquer dispositivo hospedado ou terceirizado em provedores de serviços externos, se esse equipamento estiver no domínio "<Nome da Empresa>.com" ou parecer ser de propriedade da <Nome da Empresa>.

Todo o equipamento novo que se enquadre no escopo desta política deve ser configurado de acordo com os documentos de configuração referenciados, a menos que uma dispensa seja obtida do Infosec. Todo o equipamento existente e futuro implantado nas redes não confiáveis da <Nome da Empresa> deve estar em conformidade com esta política.

**4. Política**

**4.1 Propriedade e Responsabilidades
Os equipamentos e aplicativos no escopo desta política devem ser administrados por grupos de suporte aprovados pelo Infosec para o gerenciamento de sistemas, aplicativos e redes da DMZ.

Os grupos de suporte serão responsáveis pelo seguinte:

•	O equipamento deve ser documentado no sistema de gerenciamento empresarial da empresa. No mínimo, as seguintes informações são necessárias:
o	Contatos e localização do host.
o	Hardware e sistema operacional/versão.
o	Funções principais e aplicativos.
o	Grupos de senhas para senhas privilegiadas.
•	As interfaces de rede devem ter registros apropriados do Sistema de Nomes de Domínio (DNS) (mínimo de registros A e PTR).
•	Os grupos de senhas devem ser mantidos de acordo com o sistema/processo de gerenciamento de senhas corporativas.
•	Acesso imediato aos equipamentos e registros do sistema deve ser concedido aos membros do Infosec mediante demanda, de acordo com a Política de Auditoria.
•	Mudanças nos equipamentos existentes e implantação de novos equipamentos devem seguir e governar processos/procedimentos de gerenciamento de mudanças corporativas. 

Para verificar a conformidade com esta política, o Infosec auditará periodicamente os equipamentos da DMZ de acordo com a Política de Auditoria.

**4.2 Política Geral de Configuração
Todo o equipamento deve cumprir a seguinte política de configuração:

•	Hardware, sistemas operacionais, serviços e aplicativos devem ser aprovados pelo Infosec como parte da fase de revisão pré-implantação.
•	A configuração do sistema operacional deve ser feita de acordo com os padrões seguros de instalação e configuração de host e roteador [Inserir uma referência a quaisquer padrões que você tenha].
•	Todas as correções/atualizações recomendadas pelo fornecedor de equipamentos e pelo Infosec devem ser instaladas. Isso se aplica a todos os serviços instalados, mesmo que esses serviços possam estar temporariamente ou permanentemente desativados. Grupos proprietários administrativos devem ter processos para se manterem atualizados sobre correções/atualizações apropriadas.
•	Serviços e aplicativos que não atendam aos requisitos comerciais devem ser desativados.
•	Relacionamentos de confiança entre sistemas só podem ser introduzidos de acordo com requisitos comerciais, devem ser documentados e devem ser aprovados pelo Infosec.
•	Serviços e aplicativos que não se destinam ao acesso geral devem ser restritos por listas de controle de acesso.
•	Serviços ou protocolos inseguros (conforme determinado pelo Infosec) devem ser substituídos por equivalentes mais seguros, sempre que disponíveis.
•	A administração remota deve ser realizada por canais seguros (por exemplo, conexões de rede criptografadas usando SSH ou IPSEC) ou acesso à console independente das redes da DMZ. Quando uma metodologia para conexões de canal seguro não estiver disponível, senhas únicas devem ser usadas para todos os níveis de acesso.
•	Todas as atualizações de conteúdo do host devem ocorrer por canais seguros.
•	Eventos relacionados à segurança devem ser registrados e trilhas de auditoria devem ser salvas em registros aprovados pelo Infosec. Eventos relacionados à segurança incluem (mas não estão limitados a) o seguinte:
o	Falhas no login do usuário.
o	Falha em obter acesso privilegiado.
o	Violações da política de acesso.
•	O Infosec avaliará os pedidos de dispensa de não conformidade caso a caso e aprovará as dispensas, se justificadas.

**4.3 Novas Instalações e Procedimentos de Gerenciamento de Mudanças
Todas as novas instalações e mudanças na configuração de equipamentos e aplicativos existentes devem seguir as seguintes políticas

/procedimentos:

•	As novas instalações devem ser realizadas por meio do Processo de Implantação de Equipamentos da DMZ.
•	As mudanças de configuração devem seguir os Procedimentos de Gerenciamento de Mudanças Corporativas.
•	O Infosec deve ser convidado para realizar auditorias de sistemas/aplicativos antes da implantação de novos serviços.
•	O Infosec deve ser envolvido, diretamente ou por meio de CM, para aprovar todas as novas implantações e mudanças de configuração.

**4.4 Equipamentos Terceirizados para Prestadores de Serviços Externos
A responsabilidade pela segurança dos equipamentos implantados por provedores de serviços externos deve ser esclarecida no contrato com o provedor de serviços e os contatos de segurança, e os procedimentos de escalonamento devem ser documentados. Os departamentos de contratação são responsáveis pelo cumprimento de terceiros com esta política.

**5. Conformidade com a Política**
**5.1 Medição da Conformidade**
A equipe de Infosec verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas, e feedback para o proprietário da política.

**5.2 Exceções**
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Infosec.

**5.3 Não Conformidade**
Um funcionário encontrado violando esta política pode estar sujeito a ações disciplinares, incluindo a rescisão do emprego. Provedores de serviços externos que violarem esta política podem estar sujeitos a penalidades financeiras, incluindo a rescisão de contrato.

**6. Normas, Políticas e Processos Relacionados**
•	Processo de Implantação de Equipamentos na DMZ
•	Política de Auditoria

**7. Definições e Termos**
As definições e termos a seguir podem ser encontrados no Glossário do SANS localizado em:
https://www.sans.org/security-resources/glossary-of-terms/
•	DMZ
•	Canal Seguro
•	Rede Não Confiável

**8. Histórico de Revisões**
**Data da Alteração** **Responsável** **Resumo da Alteração**
Dezembro de 2013 **Equipe de Políticas SANS** **Convertido para novo formato e retirado.**
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.