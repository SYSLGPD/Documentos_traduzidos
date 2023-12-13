# Política de Segurança de Aplicações Web

**Status da Última Atualização:** Atualizada em outubro de 2022

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todos ou partes desta política podem ser livremente utilizados pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

## 1. Visão Geral

As vulnerabilidades de aplicações web representam a maior parte dos vetores de ataque fora de malware. É crucial que qualquer aplicação web seja avaliada quanto a vulnerabilidades e que quaisquer vulnerabilidades sejam remediadas antes da implantação em produção.

## 2. Propósito

O propósito desta política é definir avaliações de segurança de aplicações web dentro da <Nome da Empresa>. As avaliações de segurança de aplicações web são realizadas para identificar fraquezas potenciais ou reais decorrentes de configurações inadvertidamente incorretas, autenticação fraca, tratamento insuficiente de erros, vazamento de informações sensíveis, etc. A descoberta e subsequente mitigação dessas questões limitarão a superfície de ataque dos serviços disponíveis da <Nome da Empresa>, tanto internamente quanto externamente, e satisfarão o cumprimento de quaisquer políticas relevantes em vigor.

## 3. Abrangência

Esta política abrange todas as avaliações de segurança de aplicações web solicitadas por qualquer indivíduo, grupo ou departamento com o propósito de manter a postura de segurança, cumprimento, gerenciamento de riscos e controle de mudanças das tecnologias em uso na <Nome da Empresa>.

Todas as avaliações de segurança de aplicações web serão realizadas por pessoal de segurança delegado, seja empregado ou contratado pela <Nome da Empresa>. Todas as descobertas são consideradas confidenciais e devem ser distribuídas para pessoas com base na necessidade de conhecimento. A distribuição de quaisquer descobertas fora da <Nome da Empresa> é estritamente proibida, a menos que aprovada pelo Chief Information Officer (CIO).

Quaisquer relações dentro de aplicações em vários níveis encontradas durante a fase de escopo serão incluídas na avaliação, a menos que explicitamente limitadas. Limitações e justificativas subsequentes serão documentadas antes do início da avaliação.

## 4. Política

### 4.1 As aplicações web estão sujeitas a avaliações de segurança com base nos seguintes critérios:

- #### 4.1.1 Lançamento de Aplicação Nova ou Importante - estará sujeito a uma avaliação completa antes da aprovação da documentação de controle de mudanças e/ou implantação no ambiente de produção.
- #### 4.1.2 Aplicação Web de Terceiros ou Adquirida - estará sujeita a uma avaliação completa, após a qual deverá cumprir os requisitos da política.
- #### 4.1.3 Lançamentos de Atualização - estarão sujeitos a um nível apropriado de avaliação com base no risco das alterações na funcionalidade e/ou arquitetura da aplicação.
- #### 4.1.4 Lançamentos de Patch - estarão sujeitos a um nível apropriado de avaliação com base no risco das alterações na funcionalidade e/ou arquitetura da aplicação.
- #### 4.1.5 Lançamentos de Emergência - um lançamento de emergência poderá ser isento de avaliações de segurança e carregará o risco presumido até que uma avaliação adequada possa ser realizada. Os lançamentos de emergência serão designados como tais pelo Chief Information Officer ou por um gerente apropriado a quem tenha sido delegada essa autoridade.
- #### 4.1.6 Revisão Anual - todas as aplicações estarão sujeitas a uma revisão anual completa em sua totalidade para avaliar os riscos potenciais da funcionalidade e/ou arquitetura.

### 4.2 Todas as questões de segurança descobertas durante as avaliações devem ser mitigadas com base nos seguintes níveis de risco. Os Níveis de Risco são baseados na Metodologia de Classificação de Risco da OWASP. Serão necessários testes de validação da remediação para confirmar a correção e/ou estratégias de mitigação para quaisquer questões descobertas de nível Médio de risco ou superior.

- #### 4.2.1 Alto - Qualquer questão de alto risco deve ser corrigida imediatamente ou outras estratégias de mitigação devem ser implementadas para limitar a exposição antes da implantação. Aplicações com questões de alto risco podem ser tiradas do ar ou negadas a liberação no ambiente de produção.
- #### 4.2.2 Médio - Questões de médio risco devem ser revisadas para determinar o que é necessário para mitigá-las e programadas de acordo com isso. Aplicações com questões de médio risco podem ser tiradas do ar ou negadas a liberação no ambiente de produção com base no número de questões e se várias questões aumentam o risco a um nível inaceitável. As questões devem ser corrigidas em uma atualização de patch ou versão, a menos que outras estratégias de mitigação limitem a exposição.
- #### 4.2.3 Baixo - A questão deve ser revisada para determinar o que é necessário para corrigir o problema e agendada de acordo com isso.

### 4.3 Os seguintes níveis de avaliação de segurança de aplicações web devem ser estabelecidos pela organização InfoSec ou por outra organização designada que realizará as avaliações.

- #### 4.3.1 Completa - Uma avaliação completa consiste em testes de todas as vulnerabilidades conhecidas de aplicações web, usando ferramentas automatizadas e manuais com base no Guia de Testes da OWASP. Uma avaliação completa utilizará técnicas manuais de teste de penetração para validar as vulnerabilidades descobertas a fim de determinar o risco geral de qualquer uma delas.
- #### 4.3.2 Rápida - Uma avaliação rápida consistirá em uma verificação automatizada (geralmente) da aplicação em busca dos dez principais riscos de segurança de aplicações web da OWASP no mínimo.
- #### 4.3.3 Direcionada - Uma avaliação direcionada é realizada para verificar alterações de remediação de vulnerabilidades ou novas funcionalidades da aplicação.

### 4.4 As ferramentas de avaliação de segurança de aplicações web atualmente aprovadas em uso e que serão utilizadas para testes são:

- <Ferramenta/Aplicação 1>
- <Ferramenta/Aplicação 2>
- ...

Outras ferramentas e/ou técnicas podem ser utilizadas dependendo do que for encontrado na avaliação padrão e da necessidade de determinar validade e risco, sujeitas à discrição da equipe de Engenharia de Segurança.

## 5. Conformidade com a Política

### 5.1 Medição da Conformidade
A equipe de InfoSec verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada pela equipe de InfoSec antecipadamente.

### 5.3 Não Conformidade
Um funcionário que violar esta política pode estar sujeito a ação disciplinar, incluindo a rescisão do emprego. As avaliações de segurança de aplicações web são um requisito do processo de controle de mudanças e devem aderir a esta política, a menos que sejam consideradas isentas. Todos os lançamentos de aplicações web devem passar pelo processo de controle de mudanças. Qualquer aplicação web que não cumpra esta política pode ser retirada do ar até que uma avaliação formal possa ser realizada a critério do Chief Information Officer.

## 6. Normas, Políticas e Processos Relacionados

- Projeto OWASP Top Ten
- Guia de Testes OWASP
- Metodologia de Classificação de Risco OWASP

## 7. Definições e Termos

Nenhum

## 8. Histórico de Revisões

Data da Alteração | Responsável | Resumo da Alteração
--- | --- | ---
Junho de 2014 | Equipe de Políticas da SANS | Atualizada e convertida para o novo formato.
Outubro de 2022 | Equipe de Políticas da SANS | Convertida para o novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.