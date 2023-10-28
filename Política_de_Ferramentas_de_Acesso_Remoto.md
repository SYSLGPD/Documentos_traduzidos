# Política de Ferramentas de Acesso Remoto

**Status da Última Atualização:** Atualizado em outubro de 2022

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todos ou partes desta política podem ser livremente utilizados pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

O software de desktop remoto, também conhecido como ferramentas de acesso remoto, oferece uma maneira para os usuários de computadores e a equipe de suporte compartilharem telas, acessarem sistemas de computadores de trabalho de casa e vice-versa. Exemplos desse tipo de software incluem LogMeIn, GoToMyPC e o Windows Remote Desktop (RDP). Embora essas ferramentas possam economizar tempo e dinheiro significativos eliminando a necessidade de viagens e permitindo a colaboração, elas também fornecem uma porta dos fundos para a rede da <Nome da Empresa> que pode ser usada para roubo, acesso não autorizado ou destruição de ativos. Como resultado, somente ferramentas de acesso remoto aprovadas, monitoradas e adequadamente controladas podem ser usadas nos sistemas de computadores da <Nome da Empresa>.

## 2. Propósito

Esta política define os requisitos para as ferramentas de acesso remoto usadas na <Nome da Empresa>.

## 3. Abrangência

Esta política se aplica a todo acesso remoto em que um dos extremos da comunicação termina em um ativo de computador da <Nome da Empresa>.

## 4. Política

Todas as ferramentas de acesso remoto usadas para comunicação entre os ativos da <Nome da Empresa> e outros sistemas devem cumprir os seguintes requisitos da política.

### 4.1 Ferramentas de Acesso Remoto

A <Nome da Empresa> fornece mecanismos para colaboração entre usuários internos, com parceiros externos e de sistemas não pertencentes à <Nome da Empresa>. A lista de software aprovado pode ser obtida em <link-para-lista-de-software-de-acesso-remoto-aprovado>. Como a configuração adequada é importante para o uso seguro dessas ferramentas, procedimentos de configuração obrigatórios são fornecidos para cada uma das ferramentas aprovadas.

A lista de software aprovado pode ser alterada a qualquer momento, mas os seguintes requisitos serão usados para selecionar produtos aprovados:

#### 4.1.1 Todas as ferramentas ou sistemas de acesso remoto que permitem a comunicação com os recursos da <Nome da Empresa> a partir da Internet ou de sistemas de parceiros externos devem exigir autenticação de múltiplos fatores. Exemplos incluem tokens de autenticação e cartões inteligentes que exigem um PIN ou senha adicional.

#### 4.1.2 A fonte do banco de dados de autenticação deve ser o Active Directory ou LDAP, e o protocolo de autenticação deve envolver um protocolo de desafio-resposta que não seja suscetível a ataques de repetição, como o OAuth 2.0. A ferramenta de acesso remoto deve autenticar mutuamente ambos os lados da sessão.

#### 4.1.3 As ferramentas de acesso remoto devem suportar o proxy de camada de aplicativo da <Nome da Empresa> em vez de conexões diretas através dos firewalls de perímetro.

#### 4.1.4 As ferramentas de acesso remoto devem oferecer suporte a criptografia forte de ponta a ponta dos canais de comunicação de acesso remoto, conforme especificado na política de protocolos de criptografia de rede da <Nome da Empresa>.

#### 4.1.5 Todos os sistemas de antivírus, prevenção de perda de dados e outros sistemas de segurança da <Nome da Empresa> não devem ser desativados, interferidos ou contornados de forma alguma.

Todas as ferramentas de acesso remoto devem ser adquiridas por meio do processo padrão de aquisição da <Nome da Empresa>, e o grupo de tecnologia da informação deve aprovar a compra.

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade

A equipe de Segurança da Informação verificará o cumprimento desta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.

### 5.2 Exceções

Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação.

### 5.3 Não Conformidade

Um funcionário que violar esta política pode estar sujeito a ação disciplinar, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados

Nenhum.

## 7. Definições e Termos

A seguinte definição e termos podem ser encontrados no Glossário da SANS localizado em:
[https://www.sans.org/security-resources/glossary-of-terms/](https://www.sans.org/security-resources/glossary-of-terms/)

- Proxy de camada de aplicativo

## 8. Histórico de Revisão

| Data da Alteração | Responsável | Resumo da Alteração |
|-------------------|------------|-----------------------|
| Junho de 2014 | Equipe de Políticas da SANS | Atualizada e convertida para o novo formato.
| Outubro de 2022 | Equipe de Políticas da SANS | Convertida para o novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.