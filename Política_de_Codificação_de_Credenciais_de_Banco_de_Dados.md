# Política de Codificação de Credenciais de Banco de Dados

## 1. Visão Geral

Credenciais de autenticação de banco de dados são uma parte necessária para autorizar um aplicativo a se conectar a bancos de dados internos. No entanto, a utilização inadequada, o armazenamento incorreto e a transmissão descuidada dessas credenciais podem resultar na exposição de ativos altamente sensíveis da <Nome da Empresa>, tornando-se um ponto de partida potencial para incidentes mais amplos dentro da organização.

## 2. Propósito

Esta política estabelece os requisitos para o armazenamento seguro e a recuperação de nomes de usuário e senhas (ou seja, as credenciais) de um banco de dados em funcionamento em uma das redes da <Nome da Empresa>. Essas credenciais serão utilizadas por um sistema que requer acesso ao banco de dados.

Os aplicativos de software em execução nas redes da <Nome da Empresa> podem necessitar de acesso a diversos servidores de banco de dados internos. A fim de estabelecer uma conexão segura e confiável, o programa deve seguir os procedimentos de autenticação, apresentando credenciais válidas para obter autorização de acesso. Caso ocorra, a manipulação inadequada dessas credenciais, a empresa estará sujeita a uma grave ameaça, levando em consideração o risco de possíveis violações dos bancos de dados envolvidos.

## 3. Abrangência

Esta política é direcionada aos implementadores de sistemas e/ou engenheiros de software que atuam na codificação de aplicativos que terão acesso a um servidor de banco de dados de produção na Rede da <Nome da Empresa>. Esta política abrange todos os softwares (programas, módulos, bibliotecas ou APIs) que precisam acessar algum banco de dados da produção de multiusuário da empresa.  Ressalta-se a recomendação de que requisitos semelhantes sejam aplicados a servidores não-produtivos e ambientes de teste, uma vez que nem sempre empregam informações sanitizadas.

## 4. Política

### 4.1 Geral

#### 4.1.1 
No intuito de zelar pela segurança dos bancos de dados internos da <Nome da Empresa>, o acesso realizado pelos programas de software devem apenas ser concedido após autenticação com credenciais. Ao serem utilizadas, não deve residir no corpo principal de execução do código-fonte do programa em texto não criptografado ou criptografia facilmente reversível. As credenciais do banco de dados não podem ser armazenadas em um local que possa ser acessado através de um servidor da web.Os Algoritmos em uso precisam atender aos padrões definidos para uso na publicação NIST FIPS 140-2 ou qualquer documento substituível, conforme a data de implementação. A utização dos algoritmos de criptografia RSA e Elliptic Curve Cryptography (ECC) é fortemente recomendado para criptografia assimétrica.

### 4.2 Requisitos Específicos

#### 4.2.1 Armazenamento de Nomes de Usuário e Senhas do Banco de Dados

- Nomes de usuário e senhas de banco de dados podem ser armazenados em um arquivo separado do corpo principal em execução do código do programa. Este arquivo não deve ser acessível para leitura ou escrita por qualquer fonte externa do programa.
- As credenciais do banco de dados podem residir no mesmo servidor que os dados. Nesse caso, é permitido armazenar um número de função de hash identificando as credenciais no corpo em execução do código do programa.
- As credenciais do banco de dados podem ser armazenadas como parte de um servidor de autenticação (ou seja, um diretório de privilégios), como um servidor LDAP usado para identificação de usuários. A autenticação do banco de dados pode ocorrer em nome de um programa como parte do processo de validação do usuário no servidor de autenticação. Nesse caso, não há necessidade de uso programático das credenciais do banco de dados.
- As credenciais do banco de dados não devem estar localizadas na árvore de documentos de um servidor da web.
- Senhas ou frases de acesso a um banco de dados devem estar em conformidade com a **Política de Senhas**.

#### 4.3 Recuperação de Nomes de Usuário e Senhas do Banco de Dados

##### 4.3.1 
Caso sejam armazenados em um arquivo que não é código-fonte, os nomes de usuário e senhas devem ser lidos do arquivo imediatamente antes de sua utilização. Imediatamente após a autenticação no banco de dados, os espaços na memória que foi registrado o nome de usuário e a senha precisam ser liberadas ou apagadas.

##### 4.3.2 
A região destinada ao armazenamento das credenciais do banco de dados deve ser fisicamente segregada das demais áreas do seu código. Em outras palavras, as credenciais devem ser mantidas em um arquivo de origem independente. Este arquivo, que contém exclusivamente as credenciais (ou seja, nome de usuário e senha), não deve incluir nenhum outro código, além das funções, rotinas ou métodos que serão utilizados para acessar essas credenciais.

##### 4.3.3 
Para linguagens que executam a partir do código-fonte, o arquivo de origem das credenciais não deve residir no mesmo diretório da árvore de diretórios navegável ou executável em que reside o corpo em execução do código.

### 4.4 Acesso a Nomes de Usuário e Senhas do Banco de Dados

#### 4.4.1 
Cada programa ou conjunto de programas que implementa uma única função comercial deve possuir credenciais de banco de dados exclusivas. O compartilhamento de credenciais entre programas não é permitido.

#### 4.4.2 
Senhas de banco de dados utilizadas por programas são senhas de nível de sistema, conforme definido na Política de Senhas.

#### 4.4.3 
Os grupos de desenvolvedores devem estabelecer um processo para assegurar que as senhas do banco de dados sejam controladas e alteradas em conformidade com a Política de Senhas. Esse processo deve incorporar um método para restringir o conhecimento das senhas do banco de dados apenas aos indivíduos que realmente necessitam delas.

## 5. Conformidade com a Política

### 5.1 Medição de Conformidade
A equipe de Segurança da Informação (Infosec) verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas, e feedback ao proprietário da política.

### 5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação (Infosec).

### 5.3 Não Conformidade
Um funcionário que violar esta política poderá estar sujeito a medidas disciplinares, incluindo a rescisão do emprego. Trabalhadores temporários, contratados ou fornecedores que violem esta política podem ter seus contratos rescindidos. Qualquer código de programa ou aplicativo que não esteja em conformidade com esta política deve ser corrigido dentro de um período de 90 dias.

## 6. Normas, Políticas e Processos Relacionados

- Política de Senhas

## 7. Definições e Termos

- Credenciais
- Corpo em Execução
- Função de Hash
- LDAP
- Módulo

## 8. Histórico de Revisões

| Data da Alteração | Responsável | Resumo da Alteração |
|-------------------|------------|-----------------------|
| Junho de 2014 | Equipe de Políticas SANS | Formatado em novo modelo e feitas pequenas alterações na redação. |
| Outubro de 2022 | Equipe de Políticas SANS | Convertido para novo formato. |
| Outubro de 2023 | Equipe de Tradução IFPB | Tradução para Português do Brasil. |
| Novembro de 2023 | Equipe de Tradução IFPB | Revisão e adaptação. |
