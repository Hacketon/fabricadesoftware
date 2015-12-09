Url do artifactory:
> http://fs.inf.ufg.br:8080/artifactory/

## Criação de novos repositórios ##
[Criar 2(dois) repositórios locais no artifactory](http://fs.inf.ufg.br:8080/artifactory/webapp/repositoryconfig.html), um para release outro para snapshot.

### Repositório snapshot ###
![http://fabricadesoftware.googlecode.com/files/criarRepositorioSnapshot.png](http://fabricadesoftware.googlecode.com/files/criarRepositorioSnapshot.png)
### Repositório release ###
![http://fabricadesoftware.googlecode.com/files/criarRepositorioRelease.png](http://fabricadesoftware.googlecode.com/files/criarRepositorioRelease.png)

## Criar usuário ##
[Criar um usuário](http://fs.inf.ufg.br:8080/artifactory/webapp/users.html) com permissão de realizar deploy no repositório e outro com permissão para acessar o repositório.
### Usuário deployer ###
Assegurar que a opção **"Can Update Profile"** esta marcada.<br />
![http://fabricadesoftware.googlecode.com/files/criarUsuarioDeployer.png](http://fabricadesoftware.googlecode.com/files/criarUsuarioDeployer.png)
### Usuário viewer ###
Assegurar que a opção **"Can Update Profile"** esta DESmarcada.<br />
![http://fabricadesoftware.googlecode.com/files/criarUsuarioViewer.png](http://fabricadesoftware.googlecode.com/files/criarUsuarioViewer.png)

## Criar nova permissão ##
[Criar os acessos](http://fs.inf.ufg.br:8080/artifactory/webapp/acls.html) necessários nos repositórios aos usuários criados
### Adicionar os novos repositórios criados a permissão nova permissão ###
![http://fabricadesoftware.googlecode.com/files/addRepositorioAPermissao.png](http://fabricadesoftware.googlecode.com/files/addRepositorioAPermissao.png)
### Habilitar operações aos usuários ###
![http://fabricadesoftware.googlecode.com/files/habilitaPermissoesAoUsuario.png](http://fabricadesoftware.googlecode.com/files/habilitaPermissoesAoUsuario.png)