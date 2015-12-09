# Ambiente java #

## Build automático ##
Como ferramenta de build automático utilizaremos o [Apache Maven](http://maven.apache.org/) licençiado sob [Apache Software License](http://maven.apache.org/license.html)

## Versionador de código fonte ##
O versionador de código fonte utilizado será o [subversion](http://subversion.apache.org/) licençiado sob [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0). São conhecidos outros versionadores, contudo, devido a alta aceitação do mercado e alta integração das ferramentas, o subversion foi selecionado.

## IDE e integradores ##
Nos projetos Java serão utilizados:
  * IDEs: [Netbeans](http://netbeans.org/) ou [Eclipse](http://www.eclipse.org/)
  * [Mylyn](http://code.google.com/p/fabricadesoftware/wiki/IntegracoesMylyn) - Conecta [Eclipse](http://www.eclipse.org/) ao repositório de tarefas
  * [Cubeon](http://code.google.com/p/fabricadesoftware/wiki/IntegracoesCubeonNetbeans) - Conecta [Netbeans](http://netbeans.org/) ao repositório de tarefas

## Integração continua ##
O serviço de integração continua será mantido nos servidores da [Fábrica de Software](http://fs.inf.ufg.br/) afim de reduzirmos o custo operacional do projeto.

A maioria dos projetos da Fábrica de Software utilizam metodologias ágeis e como consequência os integrantes contribuem diariamente com atualizações, customizações e correções do sistema. Devido a dinamicidade do código fonte, é possível que em vários momentos sejam incluidos erros no projeto que não serão detectados imediatamente mas futuramente. O cenário de detecção tardia da falha é um problema, pois, quando o erro for detectado, possivelmente vários integrantes já terão contribuido para o projeto, em cima de um código falho.
A solução seria uma ferramenta de integração contínua. Essa ferramenta pode ser configurada para verificar a consistência do código fonte sempre após uma contribuição, identificando os erros e agilizando o processo de solução do problema.
O software de integração contínua selecionado é o [Hudson](http://hudson-ci.org/). O Hudson é licençiado sob MIT license. Possui em seu núcleo plugins para subversion e maven, portanto, são distribuídos com o Hudson, bastando configura-los.

## Qualidade de software ##
<sup>fonte: http://www.sonarsource.com</sup>

O serviço responsável pela análise da qualidade do código fonte será mantido nos servidores da [Fábrica de Software](http://fs.inf.ufg.br/) afim de reduzirmos o custo operacional do projeto.

Como ferramenta de qualidade de software, utilizamos o  sonar.
O Sonar é uma ferramenta opensource para gerenciamento de qualidade sob licença [LGPL](http://www.gnu.org/licenses/lgpl-2.1.html).
O sonar se integra nativamente com o maven e com vários servidores de integração continua, entre eles Hudson, Jenkins, Cruisecontrol e TeamCity. O sonar cobre os 7(sete) pilares da qualidade de código:
  * Comentários
  * Regras de código fonte
  * Possíveis erros
  * Complexidade
  * Testes unitários
  * Duplicidade
  * Arquitetura e design

e com o auxilio de plug-ins(Cada plug-in deve ser observado a licença) essa analise de qualidade pode ser extendida a outras plataformas como .Net, Php, Delphi etc.

## Gestores de repositório maven ##
<sup>fonte: http://maven.apache.org</sup>

Os gestores de repositório servem a dois propósitos:
  * Agir como meio configurável entre a organização e os repositório públicos do maven.
  * Meio de organizar os próprios artefatos produzidos pela organização.

A ferramenta de gestão de repositórios maven será mantida nos servidores da [Fábrica de Software](http://fs.inf.ufg.br/) afim de reduzirmos o custo operacional do projeto.

  * [Artifactory Open Source](http://www.jfrog.com/products.php) sob licença [LGPL-v3.0](http://www.gnu.org/licenses/lgpl-3.0.html)
    * Hospedar os próprios repositórios
    * Proxy para repositórios remotos
    * Grupos de repositórios
    * Modelo de segurança que permite customização de acessos a grupos de indivíduos quanto a indivíduos
    * Clusterização
    * Pesquisa de artefatos atravez da indexação de artefatos
    * Agendar tarefas para manutenção dos artefatos
    * Serviços disponíveis utilizando API REST
    * Geração automatica do "settings.xml"

  * [Artifactory Pro nas nuvens](https://secure.artifactoryonline.com/registration/registration.html;jsessionid=DD5C1980BF3FEB98E3488798DD656B0C?0)
    * Serviço do artifactory enterprise com suporte: $ 55.00
    * Espaço de armazenamento de 4 Gb: $10.00 + $2.50 a cada 1Gb adicional
    * Volume de transferencia de 10 Gb: $10.00 +$0.90 a cada 1Gb adicional
    * Total dos serviços: $75/mês