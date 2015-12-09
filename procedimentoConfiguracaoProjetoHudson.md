## Nova tarefa no [hudson](http://fs.inf.ufg.br:8080/hudson) ##
Ao solicitar uma nova tarefa ao [hudson](http://fs.inf.ufg.br:8080/hudson), informar o nome e o tipo de construção, como descrito na imagem abaixo.

![http://fabricadesoftware.googlecode.com/files/novoProjetoMaven.png](http://fabricadesoftware.googlecode.com/files/novoProjetoMaven.png)

## Configurar nova tarefa ##
### Descartar Construções Antigas ###
Para desocupar espaço em hardware ocupado por construções antigas, limitar o armazenamento das tais em no máximo 5(cinco), conforme imagem abaixo
![http://fabricadesoftware.googlecode.com/files/descartarConstrucoesAntigas.png](http://fabricadesoftware.googlecode.com/files/descartarConstrucoesAntigas.png)

### Habilitar o responsável do projeto ###
Habilitar o responsável pelo projeto a solicitar novas construções da tarefa no hudson, conforme imagem abaixo.
![http://fabricadesoftware.googlecode.com/files/habilitarGerenteParaIniciarNovaConstrucaoDaTarefa.png](http://fabricadesoftware.googlecode.com/files/habilitarGerenteParaIniciarNovaConstrucaoDaTarefa.png)

### Gerenciamento de Código Fonte ###
Para configurar o subversion basta informar a URL. Devido o projeto ser open source, não é necessário informações de autenticação.
![http://fabricadesoftware.googlecode.com/files/configurarSubversionTemplate.png](http://fabricadesoftware.googlecode.com/files/configurarSubversionTemplate.png)

### Disparadores de construção automática ###
Habilitar a construção de snapshot e a consulta periódica ao repositório.
![http://fabricadesoftware.googlecode.com/files/disparadorConstrucao.png](http://fabricadesoftware.googlecode.com/files/disparadorConstrucao.png)

### Notificação de E-mail ###
Informe os emails a serem disparados em caso de falha
![http://fabricadesoftware.googlecode.com/files/dispararEmailQuandoFalha.png](http://fabricadesoftware.googlecode.com/files/dispararEmailQuandoFalha.png)

### Artifactory Configuration ###
![http://fabricadesoftware.googlecode.com/files/hudsonDeployToArtifactory.png](http://fabricadesoftware.googlecode.com/files/hudsonDeployToArtifactory.png)

### Habilitar sonar ###
![http://fabricadesoftware.googlecode.com/files/habilitarSonar.png](http://fabricadesoftware.googlecode.com/files/habilitarSonar.png)