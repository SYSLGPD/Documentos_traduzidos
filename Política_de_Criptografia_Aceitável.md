# Política de Criptografia Aceitável

**Aviso de Uso Livre:** Esta política foi criada pela SANS Institute para a comunidade da Internet. Todo ou parte desta política pode ser livremente usada pela sua organização. Não é necessária aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um e-mail para policy-resources@sans.org.

**Status da Última Atualização:** Atualizado em junho de 2014

## 1. Visão Geral
Consulte o Propósito.

## 2. Propósito
O propósito desta política é fornecer orientações que limitam o uso de criptografia a algoritmos que receberam revisão pública substancial e foram comprovados como eficazes. Além disso, esta política fornece diretrizes para garantir que sejam seguidos regulamentos federais e que seja concedida autorização legal para a disseminação e uso de tecnologias de criptografia fora dos Estados Unidos da América.

## 3. Abrangência
Esta política se aplica a todos os funcionários e afiliados da <Nome da Empresa>.

## 4. Política

### **4.1 Requisitos de Algoritmo**
#### 4.1.1 Os cifradores em uso devem atender ou exceder o conjunto definido como "compatível com AES" ou "parcialmente compatível com AES" de acordo com o Catálogo de Cifras do IETF/IRTF, ou o conjunto definido para uso na publicação FIPS 140-2 do Instituto Nacional de Padrões e Tecnologia (NIST) dos Estados Unidos, ou em quaisquer documentos que o substituam de acordo com a data de implementação. O uso do Padrão de Criptografia Avançada (AES) é fortemente recomendado para criptografia simétrica.
#### 4.1.2 Os algoritmos em uso devem atender aos padrões definidos para uso na publicação FIPS 140-2 do NIST ou em qualquer documento subsequente, de acordo com a data de implementação. O uso dos algoritmos RSA e Criptografia de Curva Elíptica (ECC) é fortemente recomendado para criptografia assimétrica.
#### 4.1.3 Algoritmos de Assinatura

Algoritmo | Comprimento da Chave (mínimo) | Comentário Adicional
--- | --- | ---
ECDSA | P-256 | Considere o RFC6090 para evitar violação de patentes.
RSA | 2048 | Deve usar um esquema de preenchimento seguro. O esquema de preenchimento PKCS#7 é recomendado. É necessária a criptografia de mensagens.
LDWM | SHA256 | Consulte o Rascunho de Assinaturas Baseadas em LDWM Hash.

### 4.2 Requisitos de Função de Hash
Em geral, <Nome da Empresa> adere à Política NIST sobre Funções de Hash.

### 4.3 Acordo de Chave e Autenticação
#### 4.3.1 As trocas de chaves devem usar um dos seguintes protocolos criptográficos: Diffie-Hellman, IKE ou Diffie-Hellman de Curva Elíptica (ECDH).
#### 4.3.2 Os pontos finais devem ser autenticados antes da troca ou derivação de chaves de sessão.
#### 4.3.3 Chaves públicas usadas para estabelecer confiança devem ser autenticadas antes do uso. Exemplos de autenticação incluem transmissão via mensagem assinada criptograficamente ou verificação manual do hash da chave pública.
#### 4.3.4 Todos os servidores usados para autenticação (por exemplo, RADIUS ou TACACS) devem possuir um certificado válido assinado por um provedor confiável conhecido.
#### 4.3.5 Todos os servidores e aplicativos que usam SSL ou TLS devem possuir certificados assinados por um provedor confiável conhecido.

### 4.4 Geração de Chave
#### 4.4.1 As chaves criptográficas devem ser geradas e armazenadas de maneira segura para evitar perda, roubo ou comprometimento.
#### 4.4.2 A geração de chaves deve ser iniciada a partir de um gerador de números aleatórios padrão da indústria (RNG). Para exemplos, consulte o Anexo C do NIST: Geradores de Números Aleatórios Aprovados para o FIPS PUB 140-2.

## 5. Conformidade com a Política

### 5.1 Medição da Conformidade
A equipe de Segurança da Informação (Infosec) verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas, e feedback ao proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação (Infosec).

### 5.3 Não Conformidade
Um funcionário que violar esta política poderá estar sujeito a medidas disciplinares, incluindo a rescisão do emprego.

## 6. Normas, Políticas e Processos Relacionados
- Publicação do Instituto Nacional de Padrões e Tecnologia (NIST) FIPS 140-2,
- Política NIST sobre Funções de Hash

## 7. Definições e Termos
As definições e termos podem ser encontrados no Glossário da SANS, localizado em: https://www.sans.org/security-resources/glossary-of-terms/

- Criptografia Proprietária

## 8. Histórico de Revisões

Data da Alteração | Responsável | Resumo da Alteração
--- | --- | ---
Junho de 2014 | Equipe de Políticas da SANS | Atualizada e convertida para o novo formato.
Outubro de 2023 | Equipe de Tradução IFPB | Traduzida para Português do Brasil.
---