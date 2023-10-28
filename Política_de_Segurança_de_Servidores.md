# Política de Segurança de Servidores

**Status da Última Atualização:** Atualizada em outubro de 2022

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todos ou partes desta política podem ser livremente utilizados pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

Servidores desprotegidos e vulneráveis continuam a ser um ponto de entrada importante para atores maliciosos. Políticas de instalação de servidores consistentes, propriedade e gerenciamento de configuração são todas baseadas em fazer o básico de forma eficaz.

## 2. Propósito

O objetivo desta política é estabelecer padrões para a configuração básica de servidores internos de propriedade e/ou operados pela <Nome da Empresa>. A implementação eficaz desta política minimizará o acesso não autorizado às informações e tecnologia proprietárias da <Nome da Empresa>.

## 3. Abrangência

Todos os funcionários, contratados, consultores, temporários e outros trabalhadores da <Nome da Empresa> e suas subsidiárias devem aderir a esta política. Esta política se aplica aos equipamentos de servidor de propriedade, operados ou arrendados pela <Nome da Empresa> ou registrados em um domínio de rede interna de propriedade da <Nome da Empresa>.

Esta política especifica requisitos para equipamentos na rede interna da <Nome da Empresa>. Para a configuração segura de equipamentos externos à <Nome da Empresa> na DMZ, consulte a Política de Equipamentos da DMZ da Internet.

## 4. Política

### 4.1 Requisitos Gerais

#### 4.1.1 Todos os servidores internos implantados na <Nome da Empresa> devem ser de propriedade de um grupo operacional responsável pela administração do sistema. Guias de configuração de servidor aprovados devem ser estabelecidos e mantidos por cada grupo operacional, com base nas necessidades de negócios e aprovados pela equipe de Segurança da Informação (InfoSec). Os grupos operacionais devem monitorar a conformidade da configuração e implementar uma política de exceção adaptada ao seu ambiente. Cada grupo operacional deve estabelecer um processo para alterar os guias de configuração, que inclui revisão e aprovação pela InfoSec. Os seguintes itens devem ser atendidos:
- Os servidores devem ser registrados no sistema de gerenciamento corporativo da empresa. No mínimo, as seguintes informações são necessárias para identificar positivamente o ponto de contato:
  - Contato(s) do servidor e localização, e um contato de backup
  - Hardware e Sistema Operacional/Versão
  - Funções principais e aplicativos, se aplicável
- As informações no sistema de gerenciamento corporativo devem ser mantidas atualizadas.
- As alterações de configuração para servidores de produção devem seguir os procedimentos apropriados de gerenciamento de alterações.

#### 4.1.2 Para fins de segurança, conformidade e manutenção, pessoal autorizado pode monitorar e auditar equipamentos, sistemas, processos e tráfego de rede conforme a Política de Auditoria.

### 4.2 Requisitos de Configuração

#### 4.2.1 A configuração do sistema operacional deve estar de acordo com as diretrizes aprovadas pela equipe InfoSec.

#### 4.2.2 Serviços e aplicativos que não serão usados devem ser desativados, sempre que prático.

#### 4.2.3 O acesso aos serviços deve ser registrado e/ou protegido por métodos de controle de acesso, como um firewall de aplicação web, se possível.

#### 4.2.4 As atualizações de segurança mais recentes devem ser instaladas no sistema assim que possível, com a única exceção sendo quando a aplicação imediata interferir com os requisitos de negócios.

#### 4.2.5 Relacionamentos de confiança entre sistemas são um risco de segurança, e seu uso deve ser evitado. Não use um relacionamento de confiança quando outro método de comunicação for suficiente.

#### 4.2.6 Sempre utilize os princípios padrão de segurança com acesso mínimo necessário para realizar uma função. Não utilize privilégios de superusuário quando uma conta não privilegiada for suficiente.

#### 4.2.7 Se uma metodologia de conexão segura estiver disponível (ou seja, tecnicamente viável), o acesso privilegiado deve ser realizado por meio de canais seguros (por exemplo, conexões de rede criptografadas usando SSH ou IPSec).

#### 4.2.8 Os servidores devem ser fisicamente localizados em um ambiente controlado por acesso e seguro.

#### 4.2.9 É proibido que os servidores operem em áreas de cubículo não controladas ou não seguras.

### 4.3 Monitoramento

#### 4.3.1 Todos os eventos relacionados à segurança em sistemas críticos ou sensíveis devem ser registrados e os registros de auditoria salvos da seguinte forma:
- Todos os registros relacionados à segurança serão mantidos online por um mínimo de 1 semana.
- Backups diários incrementais em fita serão retidos por pelo menos 1 mês.
- Backups em fita completos semanais dos registros serão retidos por pelo menos 1 mês.
- Backups completos mensais serão retidos por um mínimo de 2 anos.

#### 4.3.2 Eventos relacionados à segurança serão relatados à InfoSec, que revisará os registros e relatará os incidentes à gerência de TI. Medidas corretivas serão prescritas conforme necessário. Eventos relacionados à segurança incluem, mas não se limitam a:
- Ataques de varredura de portas
- Evidência de acesso não autorizado a contas privilegiadas
- Ocorrências anômalas que não estão relacionadas a aplicativos específicos no host.

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade
A equipe Infosec verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas, e feedback para o proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe Infosec.

### 5.3 Não Conformidade
Um funcionário que violar esta política poderá estar sujeito a medidas disciplinares, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados

- Política de Auditoria
- Política de Equipamentos DMZ da Internet

## 7. Definições e Termos
As seguintes definições e termos podem ser encontrados no Glossário da SANS localizado em: https://www.sans.org/security-resources/glossary-of-terms/
- Zona Desmilitarizada (DMZ)

## 8. Histórico de Revisão

| Data da Alteração | Responsável | Resumo da Alteração |
|-------------------|------------|-----------------------|
| Junho de 2014 | Equipe de Políticas da SANS | Atualizado e convertido para novo formato.
| Outubro de 2022 | Equipe de Políticas da SANS | Atualizado e convertido para novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.