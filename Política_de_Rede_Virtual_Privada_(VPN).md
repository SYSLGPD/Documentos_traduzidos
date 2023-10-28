# Política de Rede Virtual Privada (VPN)

**Status da Última Atualização:** Retirada

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todos ou partes desta política podem ser livremente utilizados pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

Veja o Propósito.

## 2. Propósito

O objetivo desta política é fornecer diretrizes para conexões de Rede Virtual Privada (VPN) do tipo Remote Access IPSec ou L2TP para a rede corporativa da <Nome da Empresa>.

## 3. Abrangência

Esta política se aplica a todos os funcionários da <Nome da Empresa>, contratados, consultores, temporários e outros trabalhadores, incluindo todo o pessoal afiliado a terceiros que utilizam VPNs para acessar a rede da <Nome da Empresa>. Esta política se aplica a implementações de VPN direcionadas por meio de um Concentrador IPSec.

## 4. Política

Funcionários aprovados da <Nome da Empresa> e terceiros autorizados (clientes, fornecedores, etc.) podem utilizar os benefícios das VPNs, que são um serviço "gerenciado pelo usuário". Isso significa que o usuário é responsável por selecionar um Provedor de Serviços de Internet (ISP), coordenar a instalação, instalar qualquer software necessário e pagar as taxas associadas. Detalhes adicionais podem ser encontrados na Política de Acesso Remoto.

Além disso,
1. É responsabilidade dos funcionários com privilégios de VPN garantir que usuários não autorizados não tenham acesso às redes internas da <Nome da Empresa>.
2. O uso de VPN deve ser controlado usando autenticação com senha única, como um dispositivo de token ou um sistema de chave pública/privada com uma senha forte.
3. Quando conectados à rede corporativa, as VPNs forçarão todo o tráfego de e para o PC através do túnel VPN; todo o outro tráfego será bloqueado.
4. A divisão de túneis duplos (split tunneling) NÃO é permitida; apenas uma conexão de rede é permitida.
5. Os gateways VPN serão configurados e gerenciados pelos grupos operacionais de rede da <Nome da Empresa>.
6. Todos os computadores conectados às redes internas da <Nome da Empresa> via VPN ou qualquer outra tecnologia devem usar o software antivírus mais atualizado, que é o padrão corporativo (forneça o URL deste software); isso inclui computadores pessoais.
7. Os usuários de VPN serão desconectados automaticamente da rede da <Nome da Empresa> após trinta minutos de inatividade. O usuário deve então fazer login novamente para se reconectar à rede. Pings ou outros processos de rede artificiais não devem ser usados para manter a conexão aberta.
8. O concentrador VPN está limitado a um tempo absoluto de conexão de 24 horas.
9. Usuários de computadores que não são equipamentos da <Nome da Empresa> devem configurar o equipamento para cumprir as políticas de VPN e rede da <Nome da Empresa>.
10. Somente os clientes de VPN aprovados pelo Infosec podem ser usados.
11. Ao usar a tecnologia de VPN com equipamento pessoal, os usuários devem entender que suas máquinas são uma extensão de fato da rede da <Nome da Empresa e, como tal, estão sujeitas às mesmas regras e regulamentos que se aplicam ao equipamento da <Nome da Empresa, ou seja, suas máquinas devem ser configuradas para cumprir as Políticas de Segurança do Infosec.

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade
A equipe de InfoSec verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a inspeções periódicas, monitoramento por vídeo, relatórios de ferramentas de negócios, auditorias internas e externas, e feedback para o proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela Equipe de InfoSec.

### 5.3 Não Conformidade
Um funcionário que violar esta política poderá estar sujeito a medidas disciplinares, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados

- [Política de Acesso Remoto](#)

## 7. Definições e Termos

As seguintes definições e termos podem ser encontrados no Glossário da SANS localizado em [https://www.sans.org/security-resources/glossary-of-terms/](https://www.sans.org/security-resources/glossary-of-terms/).

- Concentrador IPSec

## 8. Histórico de Revisão

| Data da Alteração | Responsável | Resumo da Alteração |
|-------------------|------------|-----------------------|
| Julho de 2014 | Equipe de Políticas da SANS | Convertido para novo formato e retirado. Conteúdo relevante adicionado à Política de Acesso à Rede em geral.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.