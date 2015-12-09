# Instalação #
Nas ultimas versões do eclipse, o Mylyn é um plugin nativo, portanto, não precisa de instalação.
Contudo, se o Mylyn não estiver instalado, no Eclipse vá em "Help=>Install New Software" e no campo "Work with" informe "http://download.eclipse.org/mylyn/releases/latest" e tecle enter.
Selecione os itens na grid abaixo do campo "Work with" e prossiga até o fim seguindo o fluxo normal das telas. Ao término, reinicie o eclipse.

# Limitações #
O plugin mylyn-eclipse é um dos produtos mais completos de desenvolvimento focado em tarefas, portanto é um produto bastante completo, contudo, existem repositórios comerciais que não se conectam ao mylyn.

# Configuração Mylyn com servidor Trac #
  1. Clique em "Window => Show View => Other"
  1. Selecione "Mylyn" e clique em "Task Repository"
  1. A janela "Task Repository" será aberta, clique com o botão direito sobre ela, selecione "Add Task Repository".
  1. A janela "Add Task Repository" será exibida, selecione a opção do Trac
  1. Desmarque a opção "Anomymous" e marque a opção "save password"
  1. Informe os dados solicitados:
    * Server: Endereço da instancia Trac
    * Label: Nome/Apelido da instancia Trac
    * User ID: Usuário Trac
    * Password: Senha do usuário Trac
  1. Clique em "Validate settings" e se os dados forem válidos, clique em "finish".

# Acesso a todas tarefas ativas #
  1. Clique em "Window => Show View => Other"
  1. Selecione "Mylyn" e clique em "Task List"
  1. A janela "Task List" será exibida, clique com botao direito e selecione "New => Query"
  1. A janela "New Query" será exibida, selecione o repositório Trac adicionado e clique em next.
  1. Informe um titulo para a query em "Query Title"
  1. Selecione todos status, com excessão de "closed"
  1. Na opção "Owner" mude a opção de filtro para "is", informe seu usuário, clique em "finish", pronto, sua query esta configurada