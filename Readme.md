## Guia rápido de como usar o Git e o Github
##

**O que é o Git?**

O Git é um sistema de **controle de versão** de arquivos - *VCS (Version Control System)* - utilizado por equipes de desenvolvimento de softwares. O controle de versão é muito importante quando várias pessoas estão editando o mesmo código em diferentes partes do mesmo arquivo ou projeto, por exemplo.

O Git mantém um histórico de qual alteração foi feita em um arquivo, quem alterou, quando e por que foi realizada essa alteração, para consultas futuras.

A instalação do Git é feita localmente no computador.

Git é diferente de Github.

Documentação de referência: https://git-scm.com/doc

<br>


**Instalação do Git**

Site para download e instalação do Git: https://git-scm.com/

<br>

**O que é o Github?**

O Github hospeda projetos que usam o Git.

O Github trabalha com repositórios (diretórios/pastas onde são armazenados nossos projetos).

Compartilhar projetos, interagir e colaborar com outros desenvolvedores ao redor do mundo, criar e publicar um portifólio, também são funcionalidades do Github.


<br>
<br>

**Conceitos**

__Repositório__: diretórios/pastas onde são armazenados os arquivos/projetos <br>

<br>

__Branch__: ramificação a partir da linha cronológica principal durante o desenvolvimento de um sistema/projeto. 
Linha cronológica do desenvolvimento. <br>
![Branch](./images/branch1.png) <br>
Por exemplo, você está desenvolvendo um site em Html e CSS. Você pode fazer uma ramificação para desenvolver só o cabeçalho (head), outra para fazer o corpo (body), outra para um segundo desenvolvedor fazer um botão etc. <br>
No final, quando a funcionalidade da ramificação estiver pronta, podemos juntar (merge) a ramificação (branch) à linha do tempo do projeto principal (main/master).<br>
![Branch](./images/branch2.png) <br>
<br>
<br>

__Commit__: salva uma versão das alterações que foram feitas nos arquivos de um projeto. São as versões. São os "pontos na história”.
<br>
<br>

__Merge__: junção da ramificação (branch) à linha do tempo do projeto principal (main/master).
<br>
<br>

__Remote__: faz a conexão do repositório que está no computador com o _Github_.
<br>
<br>

__Push__: 'Empurra' os arquivos do repositório local que já receberam o _commit_ e envia para o _Github_. Publica e cria uma versão no Github. “É o _commit_ do _Github_”.
<br>
<br>

__Pull__: o contrário do push. Ele 'puxa' o que está no repositório do Github para o seu computador.
<br>
<br>
<br>

**Roteiro e Comandos**

Iniciando um novo projeto:

- criar uma pasta no computador com o nome do projeto
- clicar com o botão direito dentro da pasta criada e clicar em “Abrir com Code” (neste exemplo, usarei o VSCode)

![Abrir com Code](./images/abrircode.png)

- criar e editar um novo arquivo no VSCode chamado “Readme.md” (md é a extensão para markdown, linguagem de marcação) – o arquivo Readme.md contém uma descrição com as instruções do novo projeto

![Readme](./images/codereadme.png)

- Dentro da mesma pasta do projeto, clique com o botão direito do mouse e após em “Git Bash Here” para abrir o terminal “Git Bash”

![Git Bash](./images/gitbashhere.png)

- O terminal do Git é aberto

![Git Bash](./images/gitbash.png)




<br>
<br>


**Comandos**

*git init* – inicializa um novo repositório vazio no branch principal (master) <br>
![git init](./images/init.png) <br>
uma pasta oculta “.git” é criada no diretório (não apagar)<br>
![folder](./images/gitfolder.png) 
<br>


(master)<br>
![git init (master)](./images/init2.png)
<br>
<br>


*git add 'nome do arquivo'* – adiciona os arquivos para uma staging area (área de preparação).  OU
*git add .* – adiciona todos os arquivos para a staging area <br>

![Staging Area](./images/stagingarea.png) <br>

![git add](./images/add.png)
<br>
<br>

![git add (all)](./images/addall.png)
<br>
<br>


*git status* – mostra o status atual  <br>
![git status](./images/status.png)
<br>
<br>

*git commit -m 'mensagem'* – salva a versão do arquivo com as últimas alterações. O parâmetro -m escreve uma mensagem/informação sobre o commit. <br>
![git commit](./images/commit.png)
<br>
Obs.: o Git tem mudado a nomenclatura do Branch principal. O padrão é “master”, mas pode aparecer também como “main”.
<br>

*git branch* - alterando o branch principal de 'master' para 'main'.<br>
git branch -M 'novo_nome' – comando para renomear a Branch atual:
![git branch](./images/branchmain.png)
<br>
<br>

No Github, criar um repositório para que tudo o que estiver dentro do repositório (Git) no computador seja enviado para um repositório no Github. Assim, os arquivos do projeto ficam disponíveis no Github para serem visualizados e utilizados por outras pessoas da equipe ou outros usuários do Github. 

Após fazer o login na sua conta do Github, entrar no menu do perfil e depois em “your repositories”. Clicar em "New" para criar um novo repositório:

![Repositórios](./images/repositoriesnew.png)

![Repositórios](./images/newrepositorie.png)

Informe um nome para o repositório, defina se ele será Público ou Privado e depois clique em “Create Repository”.

![Link](./images/linkgit.png)

Copiar o link do repoisitório "https://github.com/*username*/*NovoProjeto.git*"

No Git Bash novamente, agora vamos conectar o repositório do Git com o repositório do Github:


*git remote add origin 'link.git'* - conexão do repositório local com o repositório do Github. Esse comando é executado só uma vez.<br>
![git remote](./images/remote.png)
<br>
<br>

*git push -u origin main* – o comando push envia os arquivos que receberam o commit no computador anteriormente.

*git push origin main* 
 <br>
![git push](./images/push.png)
![git push](./images/push2.png)
![git push](./images/pushbranch.png)
<br>
<br>

Atualize a página do Github. Os arquivo do projeto devem aparecer no repositório.



*git checkout* <br>
![git checkout](./images/checkout.png)
![git checkout](./images/checkoutmain.png)
<br>
<br>

*git merge* <br>
![git merge](./images/merge.png)
<br>
<br>

*git clone* <br>
![git clone](./images/clone.png)
<br>
<br>

*git pull* <br>
![git clone](./images/pull.png)
<br>
<br>

*remover* <br>
![git rm](./images/remove.png)
<br>
<br>




<!-- 
~~~bash
$ git push origin main
~~~
-->


<br>
<br>



**Links**

Git Cheatsheet: https://ndpsoftware.com/git-cheatsheet.html <br>
Guia: https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/

