Na lista de cursos, trocaremos "Ansible" por "Ansible: Infraestrutura como código". Salvaremos o arquivo **`index.html`**, visualizaremos a página e acharemos que não ficou tão interessante. Reparem que não fizemos o commit, a adição, nem nada disso, apenas editamos o código.

Por se tratar de um único arquivo, a alteração em uma linha poderia ser desfeita com "Ctrl + Z", mas imaginemos um projeto grande, em que fazemos várias alterações, e só então entendemos que não está como queremos. Teríamos que ir desfazendo-as arquivo por arquivo, ou que só percebemos que não gostamos da alteração após ter passado um dia inteiro, impossibilitando o uso do atalho?

No Git Bash, usaremos **`git status`**, o que nos traz algumas informações. É identificado que houve modificações no arquivo, que ainda não foram commitadas. Para isso, precisaríamos chamar o **`git add`**, no entanto, é indicado que, se quiséssemos descartar as alterações, poderemos chamar **`git checkout --`** seguido do que queremos desfazer.

O **`git checkout`**, portanto, serve para **navegarmos em estados do repositório**, seja por meio de branches ou desfazendo modificações no arquivo. Sendo assim, é possível executarmos **`git checkout -- {nome do arquivo}`**. Se executarmos **`git status`** novamente, não teremos nada a ser commitado, e se abrirmos o arquivo no VS Code, verificaremos que o teste foi realmente desfeito.

Porém, e se depois da alteração no título do curso no VS Code fossemos diretamente ao Git Bash e usássemos **`git add index.html`**, mas antes do commit, testássemos e víssemos que não ficou como gostaríamos? Queremos desfazer uma alteração que já foi marcada para ser commitada, então usaremos **`git status`** para verificar se o próprio Git nos traz alguma ajuda.

É exibido que há mudanças a serem commitadas, e que poderemos utilizar **`git reset HEAD`** seguido do nome do arquivo a ser desmarcado como algo que precisa passar pelo commit. Vamos fazer isso! Para este **reset**, é preciso enviar um estado, e como ele voltará para o **HEAD**, para o local de trabalho, isto é, o estado em que ainda estaremos trabalhando.

Feito isto, com **`git status`** confirmaremos que as alterações continuam ali, porém não estão mais marcadas para serem commitadas. Sendo assim, basta utilizarmos **`git checkout -- index.html`**, o que fará com que não tenhamos mais nada a ser commitado, uma vez que a alteração foi desfeita com sucesso.

Agora, imaginemos o pior dos casos: após fazermos a alteração no título do curso, a adição e o commit do arquivo, acabamos verificando que introduzimos um bug, e que este código não podia ter sido commitado. Como será que desfazemos um commit já realizado? Usando **`git log`**, teremos o hash do commit.

Iremos copiá-lo, colar na linha de comando, juntamente com **`git revert`**. Isso fará com que o commit informado seja desfeito, criando outro. Ao ser rodado, portanto, ele irá gerar um commit cuja mensagem pode ser alterada, usaremos ":x" para salvarmos e sairmos da tela. Ao fazermos **`git log`** mais uma vez, teremos dois commits, um com a alteração do nome do curso, e outro com a reversão deste.