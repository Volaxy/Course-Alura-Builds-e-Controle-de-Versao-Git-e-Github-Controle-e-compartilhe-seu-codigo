E se quisermos guardar uma parte de uma alteração para depois, como faremos? Alguma modificação no código, para voltarmos a trabalhar nela depois, sem que precisemos commitá-la ou desfazê-la?

No Git, existe um conceito denominado Stash, e por meio de **`git stash`** conseguimos salvar todas as alterações, no caso, somente o arquivo **`index.html`**, para um local temporário, sem necessidade de um commit ou de se gerar um commit para isto.

Se, após **`git stash executarmos`** **`git stash list`**, teremos uma lista de tudo que estiver salvo nestas condições.

Queremos trazer os dados armazenados pelo **`git stash`** ao diretório de trabalho. Há duas opções: executarmos **`git stash list`**, e em seguida passarmos o número da stash em **`git stash apply 0`**, aplicaremos estas modificações, porém elas continuarão na stash. Para a remoção, poderemos usar **`git stash drop`**.

No caso de querermos fazer ambas as ações ao mesmo tempo, ou seja, pegar a última alteração adicionada à stash, e já removê-la de lá, utilizaremos **`git stash pop`** que, ao ser executado, realiza o *merge* com as modificações que já temos e aplica aquelas que já estavam salvas lá. Desta vez, ao consultarmos o VS Code, teremos o código atualizado adequadamente, com o trecho alterado e salvo temporariamente sem necessidade de commit.

