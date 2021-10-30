Para salvarmos uma alteração, ou um arquivo, precisaremos que o Git monitore os arquivo, e suas mudanças.

Para monitorar um arquivo, vamos utilizar o comando `git add`.

Se tivéssemos vários arquivos, não precisaríamos colocar seus nomes um a um, bastando `git add .` para que todos os arquivos da pasta atual sejam monitorados.

Com isso, se rodarmos `git status`, desta vez teremos um retorno diferente, incluindo "Changes to committed", isto é, "mudanças a serem commitadas", ou salvas, enviadas. Inclusive, é indicado que poderíamos executar `git rm` para remover o arquivo e para que o mesmo deixe de ser monitorado, o que não queremos fazer.

Queremos salvar as alterações, e o que poderemos entender como sendo um check point para indicar que houve mudança, seria o commit, que precisa ter modificações, que já adicionamos, mas também precisa ter uma mensagem, o que criaremos agora. Por já termos adicionado as modificações a serem enviadas, executaremos simplesmente `git commit -m ""`, em que o parâmetro -m serve para passarmos uma mensagem de commit, que será incluído entre aspas.

**A boa prática pede para colocarmos mensagens descritivas, evitando que fiquem muito grandes.**