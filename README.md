# Principais Comandos de Versionamento de Códigos

* **1 - Criar o repositório remoto no Github**

  Já logado em seu perfil no github acesse Repositories:

  ![image-20210813171503004](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813171503004.png)

    Após clicar em Repositories abrirá uma página semelhante a imagem abaixo, clique em New.

  ![image-20210813171654352](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813171654352.png)

  ​	Logo, abrirá a pagina para criar seu repositório remoto no github, preencha as informações de nome do repositório (Repository name) e  descrição (Description), selecione se o repositório será público (Public) ou privado (Private) e clique em Create repository.

  ![image-20210813172046496](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813172046496.png)

* **2 - Criar o repositório local no seu computador**

	Após a realização das etapas descritas no item 2, para isso, abra os documentos de seu computador, clique com botão direito > novo > pasta e escolha o nome da pasta. Para esse caso é "Versionamento_Atv1_Senai"
	
	![image-20210813174112489](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174112489.png)
	
	Abra a pasta que você criou e dentro dela clique com o botão direito do mouse > novo > Documento de texto. de o nome do arquivo de _README.md_
	
	![image-20210813174145756](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174145756.png)

* **3 - Git Bash Here**
  Para esse passo é necessário a instalação do [Git](https://git-scm.com/).

  Com o Git já instalado em sua máquina entre na pasta criada no item anterior, dentro dela clique com o botão direito do mouse > Git Bash Here.

  ![image-20210813174205005](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174205005.png)

  Abrirá uma janela como a janela abaixo:

  ![image-20210813174254066](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174254066.png)

* **4 - Configuração do git**
	Dentro do terminal que foi aberto no ultimo passo digite o seguinte comando _git config user.name seuusuario_. Conforme a imagem abaixo:
	
	![image-20210813174621280](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174621280.png)
	
	Depois, precisamos configurar o email que cadastramos no github com o comando _git config user.email seuemail@dominio.com_. Conforme a imagem abaixo:
	
	
	
	![image-20210813174900973](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813174900973.png)
	
	É provável que abra uma pagina pedindo a autenticação, você deve fazer a autenticação para isso. Após para confirmar se seus dados estão setados corretamente digite na janela de comandos o comando _git config --list_. Conforme a imagem abaixo:
	
	![image-20210813175040053](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813175040053.png)
	
	Serão exibidos algumas configurações, incluindo seu user.name e user.email, conforme abaixo:
	
	![image-20210813175250823](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813175250823.png)
	
	Agora para sair dessa tela aperte "q".
	
* **5 - Iniciando seu repositório local / Primeiro Commit e Upload do repositório local para repositório remoto**
	O primeiro comando que executaremos é o _git init_, que vai inicializar o repositório local em nossa pasta criada, agora essa pasta  é o repositório local e, dentro dela, há outra pasta chamada .git, criada com o comando _git init_. Essa pasta está oculta.
	
	Agora, se dermos o comando _git status_ na janela de comando:
	
	![image-20210813175844920](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813175844920.png)
	
	Recebemos um retorno dizendo que o arquivo README.md está aguardado o comando _git add ._ Então damos esse comando na janela de comandos conforme abaixo:

![image-20210813180005104](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813180005104.png)

​	Após realizar esse comando, se dermos outra vez o comando _git status_ receberemos o seguinte retorno:

![image-20210813180150885](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813180150885.png)

​	O que indica que estamos prontos para realizar o commit. Para isso digitamos na janela de comandos **_git commit_** -m "sua mensagem"_ . Conforme a imagem abaixo:

![image-20210813180421121](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813180421121.png)

Após realizar esse comando podemos, podemos ver a informações sobre ele com o comando **_git log_**.

![image-20210813180809976](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813180809976.png)

Agora devemos vincular o repositório local com o repositório remoto digitando o comando **_git remote add origin link-do-repositorio-remoto_**

![image-20210813181243840](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813181243840.png)

Você pode encontrar o link do seu repositório no seguinte espaço do seu github:

![image-20210813181418835](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813181418835.png)

Após a execução do último passo, para enfim publicar seu repositório local no github você deve digitar na janela de comandos o comando **_ git push -u origin master_**

![image-20210813181826974](C:\Users\leand\AppData\Roaming\Typora\typora-user-images\image-20210813181826974.png)

E pronto, o seu repositório local já se encontra no Github :happy::cat: ​
