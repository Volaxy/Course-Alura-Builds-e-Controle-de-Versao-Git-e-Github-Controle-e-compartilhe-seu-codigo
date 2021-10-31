# Git e Github Controle e Compartilhe seu Código
Alura course on code versioning with Git and GitHub.

Course URL -> [Git e Github Controle e Compartilhe seu Código](https://www.alura.com.br/curso-online-git-github-controle-de-versao)
![Git e Github Controle e Compartilhe seu Código](https://www.alura.com.br/assets/api/share/curso-git-github-controle-de-versao.png)
***
## Useful Links
* [Git Official](https://git-scm.com/) - Site oficial do Git, contendo downloads e documentações completas de cada comando.
* [Dev Hints](https://devhints.io/#git) - Descrição de comandos básicos do git de forma fácil.
* [GitHub](https://github.com/) - Site para hospedagem de código remoto.
* [Visualizing Git](https://git-school.github.io/visualizing-git/) - Site de demonstração de **commits** e **branchs**.

## Acronyms
* VCS - (Version Control System) / Sistema de Controle de Versões

## 01 - O que é Git?

* O que são (e para que servem) sistemas de controle de versões e como eles podem ajudar o nosso fluxo de desenvolvimento.
    * Nos ajudam a manter um histórico de alterações;
    * Nos ajudam a ter controle sobre cada alteração no código;
    * Nos ajudam para que uma alteração de determinada pessoa não influencie na alteração realizada por outra;
    * Etc.
* Que com o comando git init nós conseguimos criar um repositório Git.
* Como analisar o estado do nosso repositório através do comando git status.

## 02 - Iniciando os Trabalhos
* Que um **commit** é a forma de salvar um estado ou versão do nosso código.
* Como adicionar arquivos para serem commitados com **`git add`**.
* Como commitar arquivos, utilizando o comando **`git commit`**.
* Como verificar o histórico de commits, através do **`git log`** e algumas de suas opções:
    * **`git log --oneline`**;
    * **`git log -p`**;
    * **`git log --pretty="parametros de formatação"`**;
* Como fazer o Git não monitorar arquivos, através do **.gitignore**.
* Que não devemos realizar **commit**, ou seja, salvar um estado, da nossa aplicação que não esteja funcionando.

## 03 - Compartilhando o Trabalho
* O que são repositórios remotos;
* Como criar um repositório Git sem uma cópia dos arquivos (com **`--bare`**) para ser utilizado como servidor;
* Como adicionar links para os repositórios remotos, com o comando **`git remote add`**;
* Como baixar um repositório pela primeira vez, clonando-o com o comando **`git clone`**;
* Como enviar as nossas alterações para um repositório remoto, com **`git push`**;
* Como atualizar o nosso repositório com os dados no repositório remoto, utilizando **`git pull`**;
* O que é e para que serve o **GitHub**;
* Como criar um repositório no **GitHub**;
* Como adicionar um repositório do **GitHub** como repositório remoto.

## 04 - Trabalhando em Equipe
* Que uma *branch* (ou ramo) é uma linha de commits separada, e que pode ser utilizada para desenvolver funcionalidades independentes;
* Que com branches separados, podemos evitar que o código de uma funcionalidade interfira em outra;
* Como trazer o trabalho realizado em uma branch para outra branch, como por exemplo, o **master**, através do comando **`git merge`**;
* Que o **`git merge`** gera um novo commit, informando que houve uma mescla entre duas branches;
* Como trazer os commits de uma branch para outra, com o **`git rebase`**
* Que o **`git rebase`** não gera um commit de **merge**, simplificando o nosso log;
* Como os conflitos são apresentados pelo Git;
* Como resolver os conflitos e manter apenas as alterações desejadas com o Git.

## 05 - Manipulando as Versões
* O Git pode nos ajudar a desfazer alterações que não vamos utilizar;
* Para desfazer uma alteração antes de adicioná-la para **commit** (com **`git add`**), podemos utilizar o comando **`git checkout -- <arquivos>`**;
* Para desfazer uma alteração após adicioná-la para commit, antes precisamos executar o **`git reset HEAD <arquivos>`** e depois podemos desfazê-las com **`git checkout -- <arquivos>`**;
* Para revertermos as alterações realizadas em um **commit**, o comando **`git revert`** pode ser a solução;
* O comando **`git revert`** gera um novo **commit** informando que alterações foram desfeitas;
* Para guardar um trabalho para retomá-lo posteriormente, podemos utilizar o **`git stash`**;
* Para visualizar quais alterações estão na **stash**, podemos utilizar o comando **`git stash list`**;
* Com o comando **`git stash apply <numero>`**, podemos aplicar uma alteração específica da **stash**;
* O comando **`git stash drop <numero>`** remove determinado item da stash;
* O comando **`git stash pop`** aplica e remove a última alteração que foi adicionada na **stash**;
* O **`git checkout`** serve para deixar a cópia do código da nossa aplicação no estado que desejarmos:
    * **`git checkout <branch>`** deixa o código no estado de uma **branch** com o nome **<branch>**;
    * **`git checkout <hash>`** deixa o código no estado do *commit* com o hash <hash>.