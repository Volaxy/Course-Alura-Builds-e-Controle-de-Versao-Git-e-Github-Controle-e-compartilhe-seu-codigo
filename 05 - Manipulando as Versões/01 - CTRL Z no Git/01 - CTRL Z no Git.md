Para reverter as alterações feitas em um arquivo, sem ter feito um ***CTRL*** + ***Z*** (em arquivos que foram modificados à dias ou até semanas), ou algum tipo de `git add` ou `git commit`, usamos o comando `git checkout -- FILE_NAME`.

Caso já tenha sido feito um `git add`, usamos o comando `git reset HEAD FILES_NAME` para não excluirmos o arquivo do estado de **pronto para commit**.

Para **desfazer um commit**, copiamos o **código hash** de um commit, e digitamos o comando `git revert HASH_CODE`, digitando o nome de um novo commit que será a reversão do commit anterior.