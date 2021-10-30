# Git e Github Controle e Compartilhe seu Código
Alura course on code versioning with Git and GitHub.

Course URL -> [Git e Github Controle e Compartilhe seu Código](https://www.alura.com.br/curso-online-git-github-controle-de-versao)
![Git e Github Controle e Compartilhe seu Código](https://www.alura.com.br/assets/api/share/curso-git-github-controle-de-versao.png)
***
## Useful Links
* [Git Official](https://git-scm.com/) - Site oficial do Git, contendo downloads e documentações completas de cada comando.
* [Dev Hints](https://devhints.io/#git) - Descrição de comandos básicos do git de forma fácil.
* [GitHub](https://github.com/) - Site para hospedagem de código remoto.

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
* Como adicionar arquivos para serem commitados com `*git add*`.
* Como commitar arquivos, utilizando o comando `*git commit*`.
* Como verificar o histórico de commits, através do `*git log*` e algumas de suas opções:
    * `*git log --oneline*`;
    * `*git log -p*`;
    * `*git log --pretty="parametros de formatação"*`;
* Como fazer o Git não monitorar arquivos, através do **.gitignore**.
* Que não devemos realizar **commit**, ou seja, salvar um estado, da nossa aplicação que não esteja funcionando.