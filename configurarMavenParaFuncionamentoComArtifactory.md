## Definir chave de criptografia ##
Para uso seguro de senhas do maven, é recomendado informa-las criptografadas. Definiremos uma chave de criptografia e armazenaremos em "~/.m2/settings-security.xml".

Para criptografar uma chave de criptografia, execute:
  * mvn --encrypt-master-password senha
Após o retorno da senha criptografada, armazene no arquivo "~/.m2/settings-security.xml" o seguinte conteúdo:


&lt;settingsSecurity&gt;


> > 

&lt;master&gt;

senha criptografada

&lt;/master&gt;




&lt;/settingsSecurity&gt;



ex.: supomos que a chave de criptografia seja **chave-inf**. Após executarmos: **mvn --encrypt-master-password chave-inf** uma possível criptografia para essa chave é **{97fAM2A4rl4HBcAuDN9ZKWuQnA4NH+X3gahfiQtHE+Q=}**.
Agora basta armazenar no arquivo "~/.m2/settings-security.xml" o seguinte conteúdo:


&lt;settingsSecurity&gt;



> 

&lt;master&gt;

{97fAM2A4rl4HBcAuDN9ZKWuQnA4NH+X3gahfiQtHE+Q=}

&lt;/master&gt;




&lt;/settingsSecurity&gt;



## Criptografar senhas do repositório ##
Após a definição da chave de criptografia já podemos armazenar em "~/.m2/settings.xml" nossa senhas do repositório criptografadas. O primeiro passo é criptografar a senha do repositório executando "mvn --encrypt-password senha" e armazenar a senha criptograda em "~/.m2/settings.xml" com o conteúdo:


&lt;settings&gt;


...
> 

&lt;servers&gt;


...
> > 

&lt;server&gt;


> > > 

&lt;id&gt;

repositório

&lt;/id&gt;


> > > 

&lt;username&gt;

usuario

&lt;/username&gt;


> > > 

&lt;password&gt;

senha criptografada

&lt;/password&gt;



> > 

&lt;/server&gt;


...

> 

&lt;/servers&gt;


...


&lt;/settings&gt;

