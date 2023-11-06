# Padrão de Comunicação Sem Fio

**Aviso de Uso Livre:** Este padrão foi criado pela SANS Institute para a comunidade da Internet. Todo ou parte deste padrão pode ser livremente usado pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com um novo padrão ou uma versão atualizada deste padrão, envie um e-mail para policy-resources@sans.org.

**Status da Última Atualização:** Atualizado em outubro de 2022

## 1. Visão Geral
Consulte o Propósito.

## 2. Propósito
Este padrão especifica os requisitos técnicos que os dispositivos de infraestrutura sem fio devem atender para se conectar a uma rede da empresa <Nome da Empresa>. Somente os dispositivos de infraestrutura sem fio que atendem aos requisitos especificados neste padrão ou que foram concedidos uma exceção pela equipe de Segurança da Informação(InfoSec) são aprovados para se conectar a uma rede <Nome da Empresa>.

Dispositivos de rede, incluindo, mas não se limitando a hubs, roteadores, switches, firewalls, dispositivos de acesso remoto, modems ou pontos de acesso sem fio, devem ser instalados, suportados e mantidos por uma organização de suporte aprovada pela Segurança da Informação (Infosec). Dispositivos de rede de laboratório devem estar em conformidade com a Política de Segurança de Laboratório.

## 3. Abrangência
Todos os funcionários, contratados, consultores, temporários e outros trabalhadores na empresa <Nome da Empresa> e suas subsidiárias, incluindo todo o pessoal que mantém um dispositivo de infraestrutura sem fio em nome da mesma, devem cumprir este padrão. Este padrão se aplica a dispositivos sem fio que fazem uma conexão à rede e a todos os dispositivos de infraestrutura sem fio que fornecem conectividade sem fio à rede.

A Infosec deve aprovar exceções a este padrão antecipadamente.

## 4. Política

### 4.1 Requisitos Gerais
Todos os dispositivos de infraestrutura sem fio que se conectam a uma rede <Nome da Empresa> ou fornecem acesso a informações classificadas como confidenciais, altamente confidenciais ou restrita devem:
4.1.1 Usar o Protocolo de Autenticação Extensível-Rápida com Autenticação Via Túnel Seguro (EAP-FAST), Protocolo de Autenticação Extensível Protegido (PEAP) ou Protocolo de Autenticação Extensível com Segurança da Camada de Tradução (EAP-TLS) como protocolo de autenticação;
4.1.2 Usar protocolos Temporal Key Integrity Protocol (TKIP) ou Advanced Encryption System (AES) com um comprimento mínimo de chave de 128 bits;
4.1.3 Todos os dispositivos Bluetooth devem usar o Emparelhamento Simples Seguro com criptografia ativada.

### 4.2 Requisitos para Dispositivos de Laboratório e Isolados
4.2.1 O Identificador de Conjunto de Serviço (SSID) do dispositivo de laboratório deve ser diferente do SSID do dispositivo de produção da <Nome da Empresa>;
4.2.2 A transmissão do SSID do dispositivo de laboratório deve estar desativada.

### 4.3 Requisitos para Dispositivos de Casa
Todos os dispositivos domésticos de infraestrutura sem fio que fornecem acesso direto a uma rede <Nome da empresa>, como aqueles por trás do teletrabalho ou VPN de hardware, devem aderir ao seguinte:
4.3.1 Habilitar WPA-PSK (WiFi Protected Access com Chave Pré-Compartilhada), EAP-FAST, PEAP ou EAP-TLS
4.3.2 Ao habilitar o WPA-PSK, configurar uma chave secreta compartilhada complexa (pelo menos 20 caracteres) no cliente sem fio e no ponto de acesso sem fio
4.3.3 Desativar a transmissão do SSID
4.3.4 Alterar o nome padrão do SSID
4.3.5 Alterar o login e senha padrão

## 5. Conformidade com a Política

### 5.1 Medição da Conformidade
A equipe Infosec verificará a conformidade com este padrão por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.

### 5.2 Exceções
Qualquer exceção a este padrão deve ser aprovada antecipadamente pela equipe Infosec.

### 5.3 Não Conformidade
Um funcionário que violar esta política poderá estar sujeito a medidas disciplinares, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados
- Política de Segurança de Laboratório

## 7. Definições e Termos
As seguintes definições e termos podem ser encontrados no Glossário da SANS localizado em [https://www.sans.org/security-resources/glossary-of-terms/](https://www.sans.org/security-resources/glossary-of-terms/)
- AES
- EAP-FAST
- EAP-TLS
- PEAP
- SSID
- TKIP
- WPA-PSK

## 8. Histórico de Revisões

Data da Alteração | Responsável | Resumo da Alteração
--- | --- | ---
Junho de 2014 | Equipe de Políticas da SANS | Atualizada e convertida para o novo formato.
Outubro de 2022 | Equipe de Políticas da SANS | Convertida para o novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Tradução para português do Brasil.
