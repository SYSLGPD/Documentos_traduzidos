**Política de Segurança de Laboratórios na Zona Desmilitarizada (DMZ)**

**1. Visão Geral**
Consulte o Propósito.

**2. Propósito**
Esta política estabelece requisitos de segurança da informação para todas as redes e equipamentos implantados nos laboratórios da <Nome da Empresa> localizados na "Zona Desmilitarizada" (DMZ). A adesão a esses requisitos minimizará o risco potencial para a <Nome da Empresa> devido a danos à imagem pública causados pelo uso não autorizado dos recursos da <Nome da Empresa> e pela perda de dados sensíveis/confidenciais da empresa e propriedade intelectual.

**3. Abrangência**
Redes e dispositivos de laboratórios da <Nome da Empresa> (incluindo, mas não se limitando a roteadores, switches, hosts, etc.) que estão voltados para a Internet e localizados fora dos firewalls corporativos de Internet da <Nome da Empresa> são considerados parte dos Laboratórios DMZ e estão sujeitos a esta política. Isso inclui Laboratórios DMZ nas localidades dos principais Provedores de Serviços de Internet (ISP) e locais remotos. Todos os equipamentos existentes e futuros que se enquadram no escopo desta política devem ser configurados de acordo com os documentos de referência. Esta política não se aplica aos laboratórios localizados dentro dos firewalls corporativos de Internet da <Nome da Empresa>. Os padrões para esses laboratórios são definidos na Política de Segurança de Laboratório Interno.

**4. Política**
**4.1 Propriedade e Responsabilidades**
1. Todos os novos Laboratórios DMZ devem apresentar uma justificativa de negócios com aprovação no nível de Vice-Presidente da unidade de negócios. A Equipe de Segurança da Informação deve manter as justificativas de negócios arquivadas.
2. As organizações proprietárias de laboratórios são responsáveis por designar gerentes de laboratórios, ponto de contato (POC) e POC de backup para cada laboratório. Os proprietários dos laboratórios devem manter as informações de POC atualizadas com a Equipe de Segurança da Informação [e o sistema corporativo de gerenciamento de empresas, se existir]. Os gerentes de laboratórios ou seus substitutos devem estar disponíveis 24 horas por dia em caso de emergências.
3. Alterações na conectividade e/ou finalidade de Laboratórios DMZ existentes e o estabelecimento de novos Laboratórios DMZ devem ser solicitados por meio de uma Organização de Suporte de Rede da <Nome da Empresa> e aprovados pela Equipe de Segurança da Informação.
4. Todas as conexões ISP devem ser mantidas por uma Organização de Suporte de Rede da <Nome da Empresa>.
5. Uma Organização de Suporte de Rede deve manter um dispositivo de firewall entre o(s) Laboratório(s) DMZ e a Internet.
6. A Organização de Suporte de Rede e a Equipe de Segurança da Informação reservam o direito de interromper as conexões de laboratório se houver alguma preocupação de segurança.
7. O Laboratório DMZ fornecerá e manterá dispositivos de rede implantados no Laboratório DMZ até o ponto de demarcação da Organização de Suporte de Rede.
8. A Organização de Suporte de Rede deve registrar todos os espaços de endereço do Laboratório DMZ e informações de contato atuais [no sistema corporativo de gerenciamento de empresas, se existir].
9. Os Gerentes de Laboratórios DMZ são os principais responsáveis por garantir que seus Laboratórios DMZ cumpram esta política.
10. Acesso imediato aos equipamentos e registros de sistemas deve ser concedido aos membros da Equipe de Segurança da Informação e da Organização de Suporte de Rede mediante solicitação, de acordo com a Política de Auditoria.
11. Contas individuais de laboratório devem ser excluídas em até três (3) dias quando o acesso não for mais autorizado. Senhas de contas em grupo devem estar em conformidade com a Política de Senhas e devem ser alteradas em até três (3) dias a partir de uma alteração na associação ao grupo.
12. A Equipe de Segurança da Informação analisará as solicitações de renúncia à não conformidade caso a caso.

**4.2 Requisitos de Configuração Gerais**
1. Recursos de produção não devem depender de recursos nas redes de Laboratórios DMZ.
2. Os Laboratórios DMZ não devem ser conectados às redes internas corporativas da <Nome da Empresa>, seja diretamente ou por meio de uma conexão sem fio.
3. Os Laboratórios DMZ devem estar em uma sala fisicamente separada de qualquer rede interna. Se isso não for possível, os equipamentos devem estar em um rack trancado com acesso limitado. Além disso, o Gerente do Laboratório deve manter uma lista de pessoas com acesso aos equipamentos.
4. Os Gerentes do Laboratório são responsáveis por cumprir as seguintes políticas relacionadas:
a. Política de Senhas
b. Política de Comunicações Sem Fio
c. Política de Laboratório
5. Os dispositivos de firewall mantidos pela Organização de Suporte de Rede devem ser configurados de acordo com os princípio de menor acesso e as necessidades de negócios do Laboratório DMZ. Todos os filtros de firewall serão mantidos pela Equipe de Segurança da Informação.
6. O dispositivo de firewall deve ser o único ponto de acesso entre o Laboratório DMZ e o restante das redes da <Nome da Empresa> e/ou a Internet. Qualquer forma de interconexão que contorne o dispositivo de firewall é estritamente proibida.
7. As configurações originais do firewall e quaisquer alterações devem ser revisadas e aprovadas pela Equipe de Segurança da Informação (incluindo configurações gerais e conjuntos de regras). A Equipe de Segurança da Informação pode exigir medidas de segurança adicionais, conforme necessário.
8. O tráfego dos Laboratórios DMZ para a rede interna da <Nome da Empresa>, incluindo o acesso VPN, está sujeito à Política de Acesso Remoto.
9. Todos os roteadores e switches não usados para testes e/ou treinamento devem estar em conformidade com os documentos de padronização de Roteadores e Switches de Laboratório DMZ.
10. Os sistemas operacionais de todos os hosts internos do Laboratório DMZ que executam Serviços de Internet devem ser configurados de acordo com os padrões de instalação e configuração segura de hosts. [Adicione um link URL para o site onde seus padrões de configuração interna estão armazenados].
11. As correções/atualizações de segurança atuais aplicáveis para aplicativos que são serviços de Internet devem ser aplicadas. Os grupos de proprietários administrativos devem ter processos em vigor para manter-se atualizados nas correções/atualizações apropriadas.
12. Todas as correções/atualizações de segurança recomendadas pelo fornecedor devem ser instaladas. Grupos de proprietários administrativos devem ter processos em vigor para manter-se atualizados nas correções/atualizações apropriadas.
13. Serviços e aplicativos que não atendem aos requisitos comerciais devem ser desativados.
14. Informações confidenciais da <Nome da Empresa> são proibidas em equipamentos em laboratórios onde pessoal não pertencente à <Nome da Empresa> tem acesso físico (por exemplo, laboratórios de treinamento), de acordo com a Política de Classificação e Proteção de Dados.
15. A administração remota deve ser realizada por meio de canais seguros (por exemplo, conexões de rede criptografadas usando SSH ou IPSEC) ou acesso ao console independente das redes de Laboratórios DMZ.

**5. Conformidade com a Política**
**5.1 Medição da Conformidade**
A Equipe de Segurança da Informação verificará a conformidade com esta política por meio de vários métodos, incluindo, entre outros, verificações periódicas, monitoramento de vídeo, relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.
**5.2 Exceções**
Qualquer exceção a esta política deve ser aprovada antecipadamente pela Equipe de Segurança da Informação.
**5.3 Não Conformidade**
Um funcionário que violar esta política poderá estar sujeito a ações disciplinares, incluindo a rescisão do emprego.

**6. Normas, Políticas e Processos Relacionados**
- Política de Auditoria
- Política de Classificação e Proteção de Dados
- Política de Laboratório
- Política de Senhas
- Política de Comunicações Sem Fio

**7. Definições e Termos**
As seguintes definições e termos podem ser encontrados no Glossário SANS localizado em: [Glossário SANS](https://www.sans.org/security-resources/glossary-of-terms/)

- **Listas de Controle de Acesso (ACLs)**
- **Zona Desmilitarizada (DMZ)**
- **Princípio de Menor Acesso**
- **Serviços de Internet**
- **Ponto de Demarcação da Organização de Suporte de Rede**
- **Gerente de Laboratório**
- **Laboratório**
- **Firewall**

**8. Histórico de Revisões**
Data da Alteração	Responsável	Sumário da Alteração
Julho de 2014	Equipe de Políticas SANS	Convertido para o novo formato e aposentado. Seções apropriadas mescladas na Política de Segurança de Laboratório.
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.