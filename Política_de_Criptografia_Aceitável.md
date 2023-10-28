Política de Criptografia Aceitável
Aviso de Uso Livre: Esta política foi criada pelo SANS Institute para a comunidade da Internet. Toda ou parte desta política pode ser livremente usada por sua organização. Não é necessário aprovação prévia. Se você deseja contribuir com uma nova política ou versão atualizada desta política, envie um e-mail para policy-resources@sans.org.
Status da Última Atualização: Atualizado em junho de 2014
1. Visão Geral
Consulte o Propósito.
2. Propósito
O objetivo desta política é fornecer orientações que limitem o uso de criptografia a algoritmos que tenham recebido uma revisão pública substancial e comprovadamente funcionem eficazmente. Além disso, esta política fornece diretrizes para garantir que as regulamentações federais sejam seguidas e que autorização legal seja concedida para a divulgação e uso de tecnologias de criptografia fora dos Estados Unidos.

3. Abrangência
Esta política se aplica a todos os funcionários e afiliados da <Nome da Empresa>.
4. Política
4.1 Requisitos de Algoritmo
4.1.1 Os cifradores em uso devem atender ou exceder o conjunto definido como "compatível com AES" ou "parcialmente compatível com AES" de acordo com o Catálogo de Cifras IETF/IRTF, ou o conjunto definido para uso na publicação do Instituto Nacional de Padrões e Tecnologia dos Estados Unidos (NIST) FIPS 140-2, ou quaisquer documentos substitutivos de acordo com a data de implementação. O uso do Padrão de Criptografia Avançada (AES) é fortemente recomendado para criptografia simétrica.
4.1.2 Os algoritmos em uso devem atender aos padrões definidos para uso na publicação do NIST FIPS 140-2 ou em qualquer documento substitutivo, de acordo com a data de implementação. O uso dos algoritmos RSA e Criptografia de Curva Elíptica (ECC) é fortemente recomendado para criptografia assimétrica.
4.1.3 Algoritmos de Assinatura

Algoritmo	Tamanho da Chave
(mínimo)	Comentário Adicional
ECDSA	P-256	Considere o RFC6090 para evitar infração de patente.
RSA	2048	Deve usar um esquema de preenchimento seguro. O esquema de preenchimento PKCS#7 é recomendado. É necessário o hash da mensagem.
LDWM	SHA256	Consulte o Rascunho de Assinaturas Baseadas em Hash LDWM.

4.2 Requisitos de Função de Hash
Em geral, a <Nome da Empresa> adere à Política do NIST sobre Funções de Hash.

4.3 Acordo de Chave e Autenticação
4.3.1 As trocas de chaves devem utilizar um dos seguintes protocolos criptográficos: Diffie-Hellman, IKE ou Diffie-Hellman de Curva Elíptica (ECDH).
4.3.2 Os pontos finais devem ser autenticados antes da troca ou derivação de chaves de sessão.
4.3.3 As chaves públicas usadas para estabelecer confiança devem ser autenticadas antes do uso. Exemplos de autenticação incluem a transmissão via mensagem assinada criptograficamente ou a verificação manual do hash da chave pública.
4.3.4 Todos os servidores usados para autenticação (por exemplo, RADIUS ou TACACS) devem ter instalado um certificado válido assinado por um provedor conhecido e confiável.
4.3.5 Todos os servidores e aplicativos que usam SSL ou TLS devem ter os certificados assinados por um provedor conhecido e confiável.

4.4 Geração de Chave
4.4.1 As chaves criptográficas devem ser geradas e armazenadas de forma segura para evitar perda, roubo ou comprometimento.
4.4.2 A geração de chaves deve ser alimentada a partir de um gerador de números aleatórios padrão da indústria (RNG). Para exemplos, consulte o Anexo C do NIST: Geradores de Números Aleatórios Aprovados para FIPS PUB 140-2.

5. Conformidade com a Política
5.1 Medição de Conformidade
A equipe de Segurança da Informação verificará a conformidade com esta política por meio de vários métodos, incluindo, mas não se limitando a relatórios de ferramentas de negócios, auditorias internas e externas e feedback ao proprietário da política.
5.2 Exceções
Qualquer exceção a esta política deve ser aprovada antecipadamente pela equipe de Segurança da Informação.
5.3 Não Conformidade
Um funcionário que violar esta política pode estar sujeito a medidas disciplinares, incluindo demissão.

6 Padrões, Políticas e Processos Relacionados
Publicação do Instituto Nacional de Padrões e Tecnologia (NIST) FIPS 140-2,
Política do NIST sobre Funções de Hash

7 Definições e Termos
As seguintes definições e termos podem ser encontrados no Glossário do SANS localizado em:
https://www.sans.org/security-resources/glossary-of-terms/
• Criptografia Proprietária

8 Histórico de Revisões
Data da Alteração	Responsável	Resumo da Alteração
Junho de 2014	Equipe de Políticas do SANS	Atualizado e convertido para o novo formato.
Outubro de 2023 Equipe de Tradução IFPB Tradução para Português do Brasil.