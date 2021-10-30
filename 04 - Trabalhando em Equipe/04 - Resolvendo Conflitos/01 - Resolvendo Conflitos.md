Logados como Ana, utilizaremos **`git merge lista`**, e o Git nos informa que existe um conflito, e que houve falha no merge automático. É recomendado que corrijamos os conflitos primeiro, e depois commitemos o resultado. Ao voltarmos ao arquivo no VS Code, há indicações coloridas referenciando o conflito do Git, mas para o caso do uso de um editor de texto que não as tenha, focaremos somente no texto, ignorando as cores.

Entre as linhas **`<<<<<<< HEAD (Current Change)`** e **=======**, estão os dados do commit atual, na **master**. E entre as linhas **=======** e **`>>>>>>> lista (Incoming Change)`**, são os dados que estamos tentando trazer da branch **lista**. Ou seja, é exibida exatamente a diferença entre ambos. E tudo que precisamos fazer para corrigir este conflito é remover as informações indesejadas, sem que haja duplicação.

Editaremos e salvaremos o arquivo, retornaremos ao Git Bash e executaremos **`git status`**, e teremos a informação de que houve uma modificação em dois lugares, na branch atual e aquela que estamos tentando unificar. Feita a correção, simplesmente utilizaremos **`git add index.html`**, e então **`git commit`** para que o commit de merge seja realizado. Desta vez, se executarmos **`git log --graph`**, teremos a indicação do merge de **lista**. Em seguida, poderemos usar **`git push local master`**.

Vamos supor que trabalhamos no mesmo lugar em que foi alterado o ramo **master**, ao commitar e enviar as alterações, somos informados de um erro.

É necessário, então, antes de enviarmos quaisquer dados e alterações, garantir que estamos trabalhando com a versão mais recente do código. Isso significa que, antes do envio, precisaremos trazer este código de volta (**`git pull local master`**). Agora, sim, será feito o merge da **master** que está no "servidor" com esta.

Existem estratégias bem específicas de quando e como criar uma branch, e podem surgir dúvidas quanto à criação de uma branch para cada funcionalidade ou feature nova.