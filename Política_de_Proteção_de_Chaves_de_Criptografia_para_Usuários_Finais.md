**Política de Proteção de Chaves de Criptografia para Usuários Finais**

**Última Atualização: Atualizado em outubro de 2022**

**Isenção de Uso Gratuito:** Esta política foi criada pelo SANS Institute para a comunidade da Internet. Você pode usar toda ou parte desta política livremente em sua organização. Não é necessário aprovação prévia. Se desejar contribuir com uma nova política ou uma versão atualizada desta política, envie um email para policy-resources@sans.org.

**1. Visão Geral**
A gestão de chaves de criptografia, se não for feita corretamente, pode levar à comprometimento e divulgação não autorizada de chaves privadas usadas para proteger dados sensíveis e, consequentemente, ao comprometimento dos dados. Embora os usuários possam entender a importância de criptografar determinados documentos e comunicações eletrônicas, eles podem não estar familiarizados com os padrões mínimos de proteção de chaves de criptografia.

**2. Propósito**
Esta política descreve os requisitos para proteger as chaves de criptografia que estão sob o controle dos usuários finais. Esses requisitos são projetados para evitar a divulgação não autorizada e o uso fraudulento subsequente. Os métodos de proteção descritos incluirão controles operacionais e técnicos, como procedimentos de backup de chaves, criptografia sob uma chave separada e o uso de hardware à prova de violação.

**3. Abrangência**
Esta política se aplica a todas as chaves de criptografia listadas abaixo e à pessoa responsável por qualquer chave de criptografia listada abaixo. As chaves de criptografia abrangidas por esta política são:
- Chaves de criptografia emitidas pela <Nome da Empresa>
- Chaves de criptografia usadas para negócios da <Nome da Empresa>
- Chaves de criptografia usadas para proteger dados de propriedade da <Nome da Empresa>

As chaves públicas contidas em certificados digitais estão especificamente isentas desta política.

**4. Política**
Todas as chaves de criptografia abrangidas por esta política devem ser protegidas para evitar sua divulgação não autorizada e uso fraudulento subsequente.

**4.1 Chaves de Criptografia de Chave Secreta**
Chaves usadas para criptografia de chave secreta, também chamada de criptografia simétrica, devem ser protegidas, pois são distribuídas para todas as partes que as utilizarão. Durante a distribuição, as chaves de criptografia simétrica devem ser criptografadas usando um algoritmo mais forte com uma chave do maior comprimento de chave autorizado na Política de Criptografia Aceitável da <Nome da Empresa>. Se as chaves forem para o algoritmo mais forte, a chave deve ser dividida, sendo que cada parte da chave é criptografada com uma chave diferente do maior comprimento de chave autorizado e cada parte criptografada é transmitida por diferentes mecanismos de transmissão. O objetivo é fornecer proteção mais rigorosa para a chave do que para os dados que são criptografados com essa chave de criptografia.

As chaves de criptografia simétrica, quando em repouso, devem ser protegidas com medidas de segurança pelo menos tão rigorosas quanto as medidas usadas para a distribuição dessa chave.

**4.2 Chaves de Criptografia de Chave Pública**
A criptografia de chave pública, ou criptografia assimétrica, usa pares de chaves pública-privada. A chave pública é enviada à autoridade de certificação para ser incluída no certificado digital emitido ao usuário final. O certificado digital está disponível para todos após a emissão. A chave privada deve estar disponível apenas para o usuário final a quem o certificado digital correspondente é emitido.

**4.2.1 Chaves de Infraestrutura de Chave Pública (PKI) da <Nome da Empresa>**
Os pares de chaves pública-privada usados pela infraestrutura de chave pública (PKI) da <Nome da Empresa> são gerados no cartão inteligente à prova de violação emitido a um usuário final individual. A chave privada associada ao certificado de identidade de um usuário final, que é usada apenas para assinaturas digitais, nunca deixará o cartão inteligente. Isso impede que a equipe de Segurança da Informação recolha qualquer chave privada associada a certificados de identidade. A chave privada associada a quaisquer certificados de criptografia, que são usados para criptografar email e outros documentos, deve ser recolhida de acordo com as políticas da <Nome da Empresa>.

O acesso às chaves privadas armazenadas em um cartão inteligente emitido pela <Nome da Empresa> será protegido por um número de identificação pessoal (PIN) conhecido apenas pelo indivíduo a quem o cartão inteligente é emitido. O software do cartão inteligente será configurado para exigir a entrada do PIN antes que qualquer chave privada contida no cartão inteligente seja acessada.

**4.2.2 Outras Chaves de Criptografia de Chave Pública**
Outros tipos de chaves podem ser gerados no software do computador do usuário final e podem ser armazenados como arquivos no disco rígido ou em um token de hardware. Se o par de chaves pública-privada for gerado em um cartão inteligente, os requisitos para proteger as chaves privadas são os mesmos que os das chaves privadas associadas à PKI da <Nome da Empresa>. Se as chaves forem geradas no software, o usuário final deverá criar pelo menos um backup dessas chaves e armazenar qualquer cópia de backup de forma segura. O usuário também deve criar uma cópia de resgate de quaisquer chaves privadas usadas para criptografar dados e entregá-la ao representante de Segurança da Informação local para armazenamento seguro.

A equipe de Segurança da Informação não recolherá quaisquer chaves privadas associadas a certificados de identidade. Todos os backups, incluindo cópias de resgate, devem ser protegidos com uma senha ou frase de acesso que esteja em conformidade com a Política de Senhas da <Nome da Empresa>. Os representantes de Segurança da Informação armazenarão e protegerão as chaves de resgate conforme descrito na Política de Prática de Certificados da <Nome da Empresa>.

**4.2.3 Chaves de Infraestrutura de Chave Pública (PKI) de Organizações Comerciais ou Externas**
Ao

 trabalhar com parceiros de negócios, o relacionamento pode exigir que os usuários finais usem pares de chaves pública-privada gerados no software do computador do usuário final. Nesses casos, os pares de chaves pública-privada são armazenados em arquivos no disco rígido do usuário final. As chaves privadas são protegidas apenas pela força da senha ou frase de acesso escolhida pelo usuário final. Por exemplo, quando um usuário final solicita um certificado digital de uma PKI comercial, como a VeriSign ou a Thawte, o navegador da web do usuário final gera o par de chaves e envia a chave pública como parte da solicitação de certificado para a AC. A chave privada permanece na loja de certificados do navegador, onde a única proteção é a senha da loja de certificados do navegador. Um navegador da web que armazena chaves privadas será configurado para exigir que o usuário insira a senha da loja de certificados sempre que uma chave privada é acessada.

**4.2.4 Pares de Chaves PGP**
Se o parceiro de negócios exigir o uso do PGP, os pares de chaves pública-privada podem ser armazenados nos arquivos do usuário no disco rígido do computador ou em um token de hardware, como uma unidade USB ou um cartão inteligente. Como a proteção das chaves privadas depende da senha no chaveamento secreto, é preferível que as chaves pública-privada sejam armazenadas em um token de hardware. O PGP será configurado para exigir a entrada da senha em cada uso das chaves privadas no chaveamento secreto.

**4.3 Armazenamento em Token de Hardware**
Os tokens de hardware que armazenam chaves de criptografia serão tratados como equipamentos sensíveis da empresa, conforme descrito na política de Segurança Física da <Nome da Empresa>, quando estiverem fora dos escritórios da empresa. Além disso, todos os tokens de hardware, cartões inteligentes, tokens USB, etc., não devem ser armazenados ou deixados conectados a nenhum computador do usuário final quando não estiverem em uso. Para usuários finais que viajam com tokens de hardware, eles não devem ser armazenados ou transportados no mesmo recipiente ou bolsa que qualquer computador.

**4.4 Números de Identificação Pessoal (PINs), Senhas e Frases de Acesso**
Todos os PINs, senhas ou frases de acesso usados para proteger chaves de criptografia devem atender aos requisitos de complexidade e comprimento descritos na Política de Senhas da <Nome da Empresa>.

**4.5 Perda e Roubo**
A perda, roubo ou divulgação não autorizada potencial de qualquer chave de criptografia abrangida por esta política deve ser relatada imediatamente à Equipe de Segurança da Informação. A equipe de Segurança da Informação orientará o usuário final sobre quais ações serão necessárias em relação à revogação de certificados ou pares de chaves pública-privada.

**5. Conformidade com a Política**

**5.1 Medição da Conformidade**
A equipe de Segurança da Informação verificará a conformidade com esta política por meio de vários métodos, incluindo, entre outros, relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.
**5.2 Exceções**
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação.
**5.3 Não Conformidade**
Um funcionário que violar esta política pode estar sujeito a ações disciplinares, incluindo a rescisão do emprego.

**6. Normas, Políticas e Processos Relacionados**
- Política de Criptografia Aceitável
- Política de Prática de Certificados
- Política de Senhas
- Política de Segurança Física

**7. Definições e Termos**
As seguintes definições e termos podem ser encontrados no Glossário SANS localizado em: [Link para o Glossário SANS]

**8. Histórico de Revisões**

Data da Alteração	Responsável	Sumário da Alteração
Junho de 2014	Equipe de Políticas SANS	Atualizado e convertido para o novo formato.
Outubro de 2022	Equipe de Políticas SANS	Atualizado e convertido para o novo formato.
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.