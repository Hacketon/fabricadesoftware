# Pré Requisitos #
  * Netbeans 6.5 ou superior

# Instalação #
A instalação usou como exemplo o netBeans em protugues.
Realize o [download](http://code.google.com/p/cubeon/) e descompacte em um local conhecido. Agora no netbeans clique no menu "Ferramentas=> Plug-ins" e a janela "Plug-ins" será exibida.
Na janela "Plug-ins" clique na aba "baixados" e em seguida em "Adicionar plug-ins", acesse o diretorio descompactado e adicione todos arquivos com extensão "nbm" e instale-os.
Após a instalação acesse o menu "janela=>cubeon" e haverá duas opções:
  * Task repositories
  * Task explorer

# Limitações #
O Cubeon somente permite acesso aos repositórios [Jira](http://www.atlassian.com/software/jira/overview) e [Trac](http://trac.edgewall.org/), contudo, para repositórios [Trac](http://trac.edgewall.org/) ele oferece funcionalidades avançadas como queries e context task.

# Configuração do cubeon com um servidor Trac #
Para integração do cubeon com um servidor Trac, são necessários dois passos de configuração:
  * configurar o servidor trac
  * adicionar o repositorio de tarefas ao cubeon

Para permitir a integração efetiva do cubeon com trac é necessário que o serviço Trac tenha instalado o plog-in XML-RPC. Para isso, basta ir na aba "admin=plug-ins" e solicitar a instalação de tais plug-ins.
O ultimo passo da configuração é configurar o serviço trac como um repositório de tarefas para o cubeon, para isso, vá em "Task Repositories" (Se não estiver sendo exibida vá em "janela => cubeon => Task Repositories") clique com o botão direito e selecione "New task repository...". Selecione "Trac repository" e clique em próximo.
Informe os dados necessários:
  1. Alias: Nome/aplido para repositório
  1. Host URL: Endereço do repositório
  1. User ID: Usuário cadastrado no repositório
  1. Password: Senha do usuário cadastrado no repositório
Dentro da TreeView será exibido o nome do seu repositório adicionado.

# Acesso a todas suas tarefas ativas #
Selecione na treeView o repositório desejado, clique com o botão direito, e selecione "New Query". Informe um nome para a query, por exemplo "Todas ativas". Clique em "Add filter" e selecione "Owner", selecione a opção "is" e informe seu usuário. Clique novamente em "Add filter" e selecione "status", selecione todos itens exibidos menos "closed" e clique em finalizar. Pronto a query esta configurada.