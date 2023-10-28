**Política de Codificação de Credenciais de Banco de Dados**

**1.0 Visão Geral**
Credenciais de autenticação de banco de dados são uma parte necessária para autorizar um aplicativo a se conectar a bancos de dados internos. No entanto, o uso, armazenamento e transmissão incorretos de tais credenciais podem levar à comprometimento de ativos muito sensíveis e servir de ponto de partida para comprometimento mais amplo dentro da organização.

**2.0 Propósito**
Esta política estabelece os requisitos para armazenar e recuperar com segurança nomes de usuário e senhas de banco de dados (ou seja, credenciais de banco de dados) para uso por um programa que acessará um banco de dados em execução em uma das redes da <Nome da Empresa>.

Aplicativos de software em execução nas redes da <Nome da Empresa> podem exigir acesso a um dos muitos servidores de banco de dados internos. Para acessar esses bancos de dados, um programa deve se autenticar no banco de dados apresentando credenciais aceitáveis. Se as credenciais forem armazenadas incorretamente, elas podem ser comprometidas, levando ao comprometimento do banco de dados.

**3.0 Abrangência**
Esta política se destina a todos os implementadores de sistemas e/ou engenheiros de software que podem estar codificando aplicativos que acessarão um servidor de banco de dados de produção na Rede da <Nome da Empresa>. Esta política se aplica a todo o software (programas, módulos, bibliotecas ou APIs) que acessará um banco de dados de produção multiusuário da <Nome da Empresa>. Recomenda-se que requisitos semelhantes estejam em vigor para servidores não-produtivos e ambientes de teste, uma vez que nem sempre usam informações sanitizadas.

**4.0 Política**

**4.1 Geral**

**4.1.1** Para manter a segurança dos bancos de dados internos da <Nome da Empresa>, o acesso por programas de software só deve ser concedido após autenticação com credenciais. As credenciais usadas para essa autenticação não devem residir no corpo principal do código-fonte do programa em texto claro ou criptografia facilmente reversível. As credenciais do banco de dados não devem ser armazenadas em um local que possa ser acessado por meio de um servidor da web. Os algoritmos em uso devem atender aos padrões definidos para uso na publicação do NIST FIPS 140-2 ou em qualquer documento subsequente, de acordo com a data de implementação. O uso dos algoritmos de criptografia RSA e Elliptic Curve Cryptography (ECC) é fortemente recomendado para criptografia assimétrica.

**4.2 Requisitos Específicos**
**4.2.1 Armazenamento de Nomes de Usuário e Senhas do Banco de Dados**
- Nomes de usuário e senhas de banco de dados podem ser armazenados em um arquivo separado do corpo principal em execução do código do programa. Este arquivo não deve ser de leitura ou gravação para o mundo.
- As credenciais do banco de dados podem residir no servidor do banco de dados. Nesse caso, um número de função de hash identificando as credenciais pode ser armazenado no corpo em execução do código do programa.
- As credenciais do banco de dados podem ser armazenadas como parte de um servidor de autenticação (ou seja, um diretório de autorização), como um servidor LDAP usado para autenticação de usuários. A autenticação do banco de dados pode ocorrer em nome de um programa como parte do processo de autenticação do usuário no servidor de autenticação. Nesse caso, não há necessidade de uso programático das credenciais do banco de dados.
- As credenciais do banco de dados não podem residir na árvore de documentos de um servidor da web.
- Senhas ou frases de acesso a um banco de dados devem estar em conformidade com a Política de Senhas.

**4.3 Recuperação de Nomes de Usuário e Senhas do Banco de Dados**

**4.3.1** Se armazenados em um arquivo que não é código-fonte, os nomes de usuário e senhas do banco de dados devem ser lidos do arquivo imediatamente antes do uso. Imediatamente após a autenticação no banco de dados, a memória que contém o nome de usuário e a senha deve ser liberada ou apagada.
**4.3.2** A área em que você pode armazenar as credenciais do banco de dados deve ser fisicamente separada das outras áreas de seu código, ou seja, as credenciais devem estar em um arquivo de origem separado. O arquivo que contém as credenciais não deve conter nenhum outro código além das credenciais (ou seja, nome de usuário e senha) e quaisquer funções, rotinas ou métodos que serão usados para acessar as credenciais.
**4.3.3** Para lingu

agens que executam a partir do código-fonte, o arquivo de origem das credenciais não deve residir no mesmo diretório da árvore de diretórios navegável ou executável em que reside o corpo em execução do código.

**4.4 Acesso a Nomes de Usuário e Senhas do Banco de Dados**

**4.4.1** Todo programa ou coleção de programas que implementam uma única função comercial deve ter credenciais de banco de dados exclusivas. O compartilhamento de credenciais entre programas não é permitido.
**4.4.2** Senhas de banco de dados usadas por programas são senhas de nível de sistema, conforme definido na Política de Senhas.
**4.4.3** Os grupos de desenvolvedores devem ter um processo para garantir que as senhas do banco de dados sejam controladas e alteradas de acordo com a Política de Senhas. Este processo deve incluir um método para restringir o conhecimento das senhas do banco de dados ao necessário.

**4.5 Técnicas de Codificação para Implementar Esta Política**
[Adicionar referências às diretrizes específicas do seu site para diferentes linguagens de codificação, como Perl, JAVA, C e/ou Cpro.]

**5.0 Cumprimento da Política**

**5.1 Medição de Cumprimento**
A equipe de Segurança da Informação verificará o cumprimento desta política por meio de vários métodos, incluindo, mas não se limitando a, relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.
**5.2 Exceções**
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação.
**5.3 Não Cumprimento**
Um funcionário que violar esta política pode estar sujeito a ação disciplinar, incluindo a rescisão do emprego.
Uma violação desta política por um trabalhador temporário, contratado ou fornecedor pode resultar na rescisão de seu contrato ou atribuição com a <Nome da Empresa>.
Qualquer código de programa ou aplicativo que violar esta política deve ser corrigido dentro de um período de 90 dias.

**6.0 Normas, Políticas e Processos Relacionados**
- Política de Senhas

**7.0 Definições e Termos**
- Credenciais
- Corpo em Execução
- Função de Hash
- LDAP
- Módulo

**8.0 Histórico de Revisões**

Data da Alteração	Responsável	Resumo da Alteração
Junho de 2014	Equipe de Políticas SANS	Formatado em novo modelo e feitas pequenas alterações na redação.
Outubro de 2022	Equipe de Políticas SANS	Convertido para novo formato.
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.