# Política de Segurança para Roteadores e Switches

**Status da Última Atualização:** Atualizado em junho de 2014

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todos ou partes desta política podem ser livremente utilizados pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

Consulte o Propósito.

## 2. Propósito

Este documento descreve uma configuração mínima de segurança necessária para todos os roteadores e switches conectados a uma rede de produção ou usados em capacidade de produção na ou em nome da <Nome da Empresa>.

## 3. Abrangência

Todos os funcionários, contratados, consultores, trabalhadores temporários e outros trabalhadores na <Nome da Empresa> e suas subsidiárias devem aderir a esta política. Todos os roteadores e switches conectados às redes de produção da <Nome da Empresa> são afetados.

## 4. Política

Cada roteador deve atender aos seguintes padrões de configuração:

1. Nenhuma conta de usuário local é configurada no roteador. Roteadores e switches devem usar o TACACS+ para autenticação de usuário.

2. A senha de habilitação no roteador ou switch deve ser mantida em uma forma criptografada segura. O roteador ou switch deve ter a senha de habilitação definida como a senha de produção atual do roteador/switch fornecida pela organização de suporte do dispositivo.

3. Os seguintes serviços ou recursos devem ser desativados:
   a. Broadcasts direcionados por IP
   b. Pacotes de entrada no roteador/switch originados com endereços inválidos, como endereços RFC1918
   c. Pequenos serviços TCP
   d. Pequenos serviços UDP
   e. Todo roteamento e comutação de origem
   f. Todos os serviços da web em execução no roteador
   g. Protocolo de descoberta da <Nome da Empresa> em interfaces conectadas à Internet
   h. Serviços Telnet, FTP e HTTP
   i. Autoconfiguração

4. Os seguintes serviços devem ser desativados, a menos que uma justificativa de negócios seja fornecida:
   a. Protocolo de descoberta da <Nome da Empresa> e outros protocolos de descoberta
   b. Troncos dinâmicos
   c. Ambientes de script, como o shell TCL

5. Os seguintes serviços devem ser configurados:
   a. Criptografia de senha
   b. NTP configurado para uma fonte padrão corporativa
6. Todas as atualizações de roteamento devem ser feitas usando atualizações de roteamento seguras.

7. Use cadeias de comunidade SNMP padronizadas pela corporação. As cadeias padrão, como "public" ou "private", devem ser removidas. O SNMP deve ser configurado para usar a versão mais segura do protocolo permitida pela combinação do dispositivo e sistemas de gerenciamento.

8. Listas de controle de acesso devem ser usadas para limitar a origem e o tipo de tráfego que pode terminar no próprio dispositivo.

9. Listas de controle de acesso para transitar o dispositivo devem ser adicionadas à medida que as necessidades de negócios surgem.

10. O roteador deve ser incluído no sistema de gerenciamento corporativo com um ponto de contato designado.

11. Cada roteador deve ter a seguinte declaração apresentada para todas as formas de login, seja remoto ou local:

   "ACESSO NÃO AUTORIZADO A ESTE DISPOSITIVO DE REDE É PROIBIDO. Você deve ter permissão explícita para acessar ou configurar este dispositivo. Todas as atividades realizadas neste dispositivo podem ser registradas, e violações desta política podem resultar em ação disciplinar e podem ser relatadas à aplicação da lei. Não há direito à privacidade neste dispositivo. O uso deste sistema constituirá consentimento para monitoramento."

12. O Telnet nunca pode ser usado em qualquer rede para gerenciar um roteador, a menos que haja um túnel seguro protegendo todo o caminho de comunicação. O SSH versão 2 é o protocolo de gerenciamento preferido.

13. Protocolos de roteamento dinâmico devem usar autenticação em atualizações de roteamento enviadas para vizinhos. A codificação da senha para a cadeia de autenticação deve ser habilitada quando suportada.

14. O padrão de configuração de roteadores corporativos definirá a categoria de dispositivos sensíveis de roteamento e comutação e exigirá serviços ou configurações adicionais em dispositivos sensíveis, incluindo:

   a. Contabilidade da lista de acesso IP
   b. Registro de dispositivos
   c. Pacotes de entrada no roteador originados com endereços inválidos, como endereços RFC1918, ou que poderiam ser usados para falsificar o tráfego de rede, devem ser descartados
   d. Acesso ao console do roteador e ao modem deve ser restrito por controles de segurança adicionais

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade

A equipe de InfoSec verificará o cumprimento desta política por meio de vários métodos, incluindo, mas não se limitando a passeios periódicos, monitoramento de vídeo, relatórios de ferramentas de negócios, auditorias internas e externas, e feedback para o proprietário da política.

### 5.2 Exceções

Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de InfoSec.

### 5.3 Não Conformidade

Um funcionário que violar esta política pode estar sujeito a ação disciplinar, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados

Nenhum.

## 7. Definições e Termos

Nenhum.

## 8. Histórico de Revisão

| Data da Alteração | Responsável | Resumo da Alteração |
|-------------------|------------|-----------------------|
| Junho de 2014 | Equipe de Políticas da SANS | Atualizada e convertida para o novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.
